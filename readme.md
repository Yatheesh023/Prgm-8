This is an explanation of the project being done

8 MINGW64 \~/Desktop/1KS25CS165 (bugfix-ui)

$ git commit -m "Added bugfix.txt"

\[bugfix-ui 8d68876] Added bugfix.txt

&#x20;1 file changed, 1 insertion(+)

&#x20;create mode 100644 bugfix.txt



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (bugfix-ui)

$ ls

Doc.txt  Hey.txt  bugfix.txt  readme.md



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (bugfix-ui)

$ git switch -c feature-login

fatal: a branch named 'feature-login' already exists



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (bugfix-ui)

$ git switch feature-login

Switched to branch 'feature-login'



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (feature-login)

$ ls

Doc.txt  Hey.txt  feature.txt  readme.md



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (feature-login)

$ git switch master

Switched to branch 'master'



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (master)

$ ls

Doc.txt  Hey.txt  readme.md



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (master)

$ git branch

&#x20; bugfix-ui

&#x20; feature-login

\* master



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (master)

$ git merge -m "merging feature login branch to main"feature login

merge: login - not something we can merge



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (master)

$ git merge -m "merging feature login branch to main" feature-login

Updating a5966ec..d2ba15a

Fast-forward (no commit created; -m option ignored)

&#x20;feature.txt | 1 +

&#x20;1 file changed, 1 insertion(+)

&#x20;create mode 100644 feature.txt



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (master)

$ ls

Doc.txt  Hey.txt  feature.txt  readme.md



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (master)

$ git log --oneline

d2ba15a (HEAD -> master, feature-login) This is my first commit

a5966ec This is my second commit

85a990c added readme.md

95fe322 This is my 1st commit



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (master)

$ git log

commit d2ba15a387c6e624ed154155eeb291adf6a54469 (HEAD -> master, feature-login)

Author: Yatheesh <yatheeshgowda205@gmail.com>

Date:   Wed Sep 16 09:18:28 2026 +0530



&#x20;   This is my first commit



commit a5966ecdaff2fdf3fbc8c68f8d75d7abfa9ee424

Author: Yatheesh <yatheeshgowda205@gmail.com>

Date:   Sat Sep 12 09:26:12 2026 +0530



&#x20;   This is my second commit



commit 85a990c7c6fbef3e9d1144679361a38d6d7e58db

Author: Yatheesh <yatheeshgowda205@gmail.com>

Date:   Sat Sep 12 09:10:58 2026 +0530



&#x20;   added readme.md



commit 95fe3222194f420addd4fff88e57a608ec44030d

Author: Yatheesh <yatheesh205@gmail.com>

Date:   Wed Sep 9 10:24:23 2026 +0530



&#x20;   This is my 1st commit



ksitnwsys31@DESKTOP-V428D38 MINGW64 \~/Desktop/1KS25CS165 (master)

$ git log --oneline --all --graph

\* 8d68876 (bugfix-ui) Added bugfix.txt

| \* d2ba15a (HEAD -> master, feature-login) This is my first commit

|/

\* a5966ec This is my second commit

\* 85a990c added readme.md

\* 95fe322 This is my 1st commit



