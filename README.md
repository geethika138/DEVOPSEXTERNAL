DELL@DESKTOP-JH7MEPQ MINGW64 ~ ((...))
$ cd /c/devops2

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2
$ ^[[200~
bash: $'\E[200~': command not found

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2
$ git --version
git version 2.49.0.windows.1

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2
$ git init
Initialized empty Git repository in C:/devops2/.git/

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git config --global user.name "geethika138"

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git config --global user.email "harshini.yalamati@sasi.ac.in"

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        form.css
        form.html

nothing added to commit but untracked files present (use "git add" to track)

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ ^C


DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git add .

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git add form.html

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git add form.css

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   form.css
        new file:   form.html


DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git commit -m "Initial commit"
[master (root-commit) bf4ad2b] Initial commit
 2 files changed, 78 insertions(+)
 create mode 100644 form.css
 create mode 100644 form.html

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git log
commit bf4ad2b2e79429b03f569f0109035c8a7a080cac (HEAD -> master)
Author: geethika138 <harshini.yalamati@sasi.ac.in>
Date:   Sun Apr 13 12:49:58 2025 +0530

    Initial commit

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git branch
* master

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git checkout dev
error: pathspec 'dev' did not match any file(s) known to git

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (master)
$ git checkout -b dev
Switched to a new branch 'dev'

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git merge dev
Already up to date.

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git remote add origin https://github.com/geethika138/devops2.git

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git remote -v
origin  https://github.com/geethika138/devops2.git (fetch)
origin  https://github.com/geethika138/devops2.git (push)

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git clone ^C

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git clone https://github.com/geethika138/devops2.git
Cloning into 'devops2'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git pull origin main
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 863 bytes | 14.00 KiB/s, done.
From https://github.com/geethika138/devops2
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git pull origin main



DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/geethika138/devops2.git'

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ ^C

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git branch
* dev
  master

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ ^C

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$  git push -u origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1002 bytes | 62.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/geethika138/devops2/pull/new/dev
remote:
To https://github.com/geethika138/devops2.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (dev)
$ git branch -m main

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ git push -u origin main
To https://github.com/geethika138/devops2.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/geethika138/devops2.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ ^C

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ ^C

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ git pull origin main --rebase
From https://github.com/geethika138/devops2
 * branch            main       -> FETCH_HEAD
Successfully rebased and updated refs/heads/main.

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.05 KiB | 63.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/geethika138/devops2.git
   f71de53..e707d25  main -> main

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ git fetch

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ git rm form.css
rm 'form.css'

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ git help status
/usr/bin/start: line 8: : command not found

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ git help
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--no-lazy-fetch]
           [--no-optional-locks] [--no-advice] [--bare] [--git-dir=<path>]
           [--work-tree=<path>] [--namespace=<name>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   restore    Restore working tree files
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   diff       Show changes between commits, commit and working tree, etc
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   backfill   Download missing objects in a partial clone
   branch     List, create, or delete branches
   commit     Record changes to the repository
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   reset      Reset current HEAD to the specified state
   switch     Switch branches
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$ ^C

DELL@DESKTOP-JH7MEPQ MINGW64 /c/devops2 (main)
$
