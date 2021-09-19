Liu Zeyuan

Commit on rebase branch:
git commit -a -m ¡°c1¡±
git commit -a -m ¡°c2¡±

Commit on develop branch:
git commit -a -m ¡°c3¡±
git commit -a -m ¡°c4¡±

Commit on develop branch after rebasing:
git checkout develop
git rebase rebase
git add helloworld.py
git rebase --continue
git add helloworld.py
git rebase ¨Ccontinue

final screenshot:

14917@LAPTOP-EQGD09Q6 MINGW64 /c/Users/14917/Desktop/UofT/ECE444/ECE444-Lab1 (develop)
$ git log
commit f7e809ded501c046f62ea7ab15f80082e3182613 (HEAD -> develop, origin/develop)
Author: yuukiasuna <louis.zy.liu@gmail.com>
Date:   Sun Sep 19 02:26:27 2021 -0400

    c4

commit 38246a18c8f6324c196280a81fcb4db042caaf86
Author: yuukiasuna <louis.zy.liu@gmail.com>
Date:   Sun Sep 19 02:26:05 2021 -0400

    c3

commit 3b26abd8434c724ea0ba10ea67a9ae644a5f3fc5 (rebase)
Author: yuukiasuna <louis.zy.liu@gmail.com>
Date:   Sun Sep 19 02:24:53 2021 -0400

    c2

commit 20da087bd69c82dd9e1adf6d0075b64c09face94
Author: yuukiasuna <louis.zy.liu@gmail.com>
Date:   Sun Sep 19 02:23:59 2021 -0400

    c1
