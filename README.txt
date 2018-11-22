
GILDAS-PC@GILDAS-PC MINGW64 ~
$ mkdir text-repository

GILDAS-PC@GILDAS-PC MINGW64 ~
$ cd text-repository

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository
$ git status
fatal: not a git repository (or any of the parent directories): .git

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository
$ git init
Initialized empty Git repository in C:/Users/GILDAS-PC/text-repository/.git/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ touch README.txt

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        README.txt

nothing added to commit but untracked files present (use "git add" to track)

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ subl README.txt

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        README.txt

nothing added to commit but untracked files present (use "git add" to track)

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add^C

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add  README.txt

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   README.txt


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git commit -m "add readme text to text repository"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'GILDAS-PC@GILDAS-PC.(none)')

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git config --global user.email "habigildas@gmail.com"

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$  git config --global user.name "gilgildas"

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git commit -m "add readme text to text repository"
[master (root-commit) 0a80d83] add readme text to text repository
 1 file changed, 1 insertion(+)
 create mode 100644 README.txt

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
nothing to commit, working tree clean

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ touch index.html

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ subl index.html

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        index.html

nothing added to commit but untracked files present (use "git add" to track)

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add  index.html

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git commit -m "add html file to my repository"
[master ebb1c76] add html file to my repository
 1 file changed, 11 insertions(+)
 create mode 100644 index.html

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
nothing to commit, working tree clean

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add -p
diff --git a/index.html b/index.html
index d93e57b..b72301d 100644
--- a/index.html
+++ b/index.html
@@ -6,6 +6,8 @@
 <body>
        <h1>my repository script</h1>
        <p>this the second file of my repository</p>
+       <h3>my repository text</h3>
+       <p>this is the file containing my text file</p>

 </body>
 </html>
\ No newline at end of file
Stage this hunk [y,n,q,a,d,e,?]? y


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   index.html


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ commit -m " adding paragraph to index.html"
bash: commit: command not found

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git commit -m " adding paragraph to index.html"
[master b039d0d]  adding paragraph to index.html
 1 file changed, 2 insertions(+)

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
nothing to commit, working tree clean

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ touch style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ subltouch style.css
bash: subltouch: command not found

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ subl  style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        style.css

nothing added to commit but untracked files present (use "git add" to track)

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   style.css


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git commit -m "add style file to repository"
[master 5b25fc1] add style file to repository
 1 file changed, 12 insertions(+)
 create mode 100644 style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
nothing to commit, working tree clean

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add -p
No changes.

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
git: 'staus' is not a git command. See 'git --help'.

The most similar command is
        status

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   style.css

no changes added to commit (use "git add" and/or "git commit -a")

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add -p
diff --git a/style.css b/style.css
index c9341e2..8f89311 100644
--- a/style.css
+++ b/style.css
@@ -1,7 +1,8 @@
 body{
        background-color: #cccccc;
        display: flex;
-
+       color: #fff;
+

 }
 h1{
Stage this hunk [y,n,q,a,d,j,J,g,/,e,?]? y
@@ -9,4 +10,8 @@ h1{
        text-align: center;

 }
+p{
+       line-height: 1.6
+}
+

Stage this hunk [y,n,q,a,d,K,g,/,e,?]? y
<stdin>:22: new blank line at EOF.
+
warning: 1 line adds whitespace errors.


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add -p
diff --git a/style.css b/style.css
index 8f89311..982c5e7 100644
--- a/style.css
+++ b/style.css
@@ -11,7 +11,7 @@ h1{

 }
 p{
-       line-height: 1.6
+       line-height: 1.6;
 }


Stage this hunk [y,n,q,a,d,e,?]? y


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   style.css


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git commit -m "changing  paragraph style  "
[master 2b5c43a] changing  paragraph style
 1 file changed, 6 insertions(+), 1 deletion(-)

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
nothing to commit, working tree clean

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git clone https://github.com/gilgildas/text-file.git
Cloning into 'text-file'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ ls
index.html  README.txt  style.css  text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ mv index.html text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ ls
README.txt  style.css  text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ mv README.txt text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ mv README.txttext-file/
mv: missing destination file operand after 'README.txttext-file/'
Try 'mv --help' for more information.

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ mv README.txt text-file/
mv: cannot stat 'README.txt': No such file or directory

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ mv README.txt text-file/
mv: cannot stat 'README.txt': No such file or directory

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ mv README.txttext-file/ text-file/
mv: cannot stat 'README.txttext-file/': No such file or directory

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ ls
style.css  text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ cd text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ ls
index.html  README.md  README.txt

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ cd

GILDAS-PC@GILDAS-PC MINGW64 ~
$ cd /text-repository
bash: cd: /text-repository: No such file or directory

GILDAS-PC@GILDAS-PC MINGW64 ~
$ cd text-repository

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ ls
style.css  text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ mv style.css text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ ls
text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ cd text-file

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ ls
index.html  README.md  README.txt  style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ cat index.html
<!DOCTYPE html>
<html>
<head>
        <title>my repository</title>
</head>
<body>
        <h1>my repository script</h1>
        <p>this the second file of my repository</p>
        <h3>my repository text</h3>
        <p>this is the file containing my text file</p>

</body>
</html>
GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ cd text-repository
bash: cd: text-repository: No such file or directory

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ cd text-repository
bash: cd: text-repository: No such file or directory

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ cd

GILDAS-PC@GILDAS-PC MINGW64 ~
$ cd text-repository

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    README.txt
        deleted:    index.html
        deleted:    style.css

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        text-file/

no changes added to commit (use "git add" and/or "git commit -a")

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   text-file/README.md
        new file:   text-file/README.txt
        new file:   text-file/index.html
        new file:   text-file/style.css

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    README.txt
        deleted:    index.html
        deleted:    style.css


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ ls
text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git commit -m "move files to text-file"
[master 5b82a4d] move files to text-file
 4 files changed, 33 insertions(+)
 create mode 100644 text-file/README.md
 create mode 100644 text-file/README.txt
 create mode 100644 text-file/index.html
 create mode 100644 text-file/style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    README.txt
        deleted:    index.html
        deleted:    style.css

no changes added to commit (use "git add" and/or "git commit -a")

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git add -p
diff --git a/README.txt b/README.txt
index dd65137..0000000
--- a/README.txt
+++ /dev/null
deleted file mode 100644
@@ -1 +0,0 @@
-my file is called README!
\ No newline at end of file
Stage deletion [y,n,q,a,d,?]? y

diff --git a/index.html b/index.html
index b72301d..0000000
--- a/index.html
+++ /dev/null
deleted file mode 100644
@@ -1,13 +0,0 @@
-<!DOCTYPE html>
-<html>
-<head>
-       <title>my repository</title>
-</head>
-<body>
-       <h1>my repository script</h1>
-       <p>this the second file of my repository</p>
-       <h3>my repository text</h3>
-       <p>this is the file containing my text file</p>
-
-</body>
-</html>
\ No newline at end of file
Stage deletion [y,n,q,a,d,?]? y

diff --git a/style.css b/style.css
index 982c5e7..0000000
--- a/style.css
+++ /dev/null
deleted file mode 100644
@@ -1,17 +0,0 @@
-body{
-       background-color: #cccccc;
-       display: flex;
-       color: #fff;
-
-
-}
-h1{
-       font-size:18px;
-       text-align: center;
-
-}
-p{
-       line-height: 1.6;
-}
-
-
Stage deletion [y,n,q,a,d,?]? y


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        deleted:    README.txt
        deleted:    index.html
        deleted:    style.css


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git commit -m "files moved to text-file"
[master fc48d54] files moved to text-file
 3 files changed, 31 deletions(-)
 delete mode 100644 README.txt
 delete mode 100644 index.html
 delete mode 100644 style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ git status
On branch master
nothing to commit, working tree clean

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ ls
text-file/

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository (master)
$ cd text-file

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        README.txt
        index.html
        style.css

nothing added to commit but untracked files present (use "git add" to track)

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git add -p
No changes.

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git add README.txt

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git add index.html

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git add style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   README.txt
        new file:   index.html
        new file:   style.css


GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git commit "files added to text-file "
error: pathspec 'files added to text-file ' did not match any file(s) known to git

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git commit  -m "files added to text-file "
[master 8a51758] files added to text-file
 3 files changed, 31 insertions(+)
 create mode 100644 README.txt
 create mode 100644 index.html
 create mode 100644 style.css

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

GILDAS-PC@GILDAS-PC MINGW64 ~/text-repository/text-file (master)
$ git push origin master
Logon failed, use ctrl+c to cancel basic credential prompt.
Username for 'https://github.com': gilgildas
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 644 bytes | 161.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0)
To https://github.com/gilgildas/text-file.git
   c365a5a..8a51758  master -> master

