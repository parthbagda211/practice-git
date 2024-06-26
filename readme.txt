Initialized empty Git repository in /home/bagda/todoapp/tasks/.git/
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git add .
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git commit -m 'added all files'
[master (root-commit) b5d2ac1] added all files
 21 files changed, 127 insertions(+)
 create mode 100644 __init__.py
 create mode 100644 __pycache__/__init__.cpython-310.pyc
 create mode 100644 __pycache__/models.cpython-310.pyc
 create mode 100644 __pycache__/repository.cpython-310.pyc
 create mode 100644 __pycache__/service.cpython-310.pyc
 create mode 100644 __pycache__/test_repository.cpython-310.pyc
 create mode 100644 __pycache__/test_service.cpython-310.pyc
 create mode 100644 __pycache__/test_views.cpython-310.pyc
 create mode 100644 __pycache__/tests.cpython-310.pyc
 create mode 100644 admin.py
 create mode 100644 apps.py
 create mode 100644 migrations/__init__.py
 create mode 100644 migrations/__pycache__/__init__.cpython-310.pyc
 create mode 100644 models.py
 create mode 100644 repository.py
 create mode 100644 service.py
 create mode 100644 test_repository.py
 create mode 100644 test_service.py
 create mode 100644 test_views.py
 create mode 100644 tests.py
 create mode 100644 views.py
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch -m branch
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch -all
error: did you mean `--all` (with two dashes)?
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch --all
* branch
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git remote add origin https://github.com/parthbagda211/nothing-much-.git
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git pus -u origin branch
git: 'pus' is not a git command. See 'git --help'.

The most similar commands are
	push
	pull
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git push -u origin branch
Username for 'https://github.com': parthbagda211
Password for 'https://parthbagda211@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/parthbagda211/nothing-much-.git/'
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git remote set-url origin git@github.com:parthbagda211/nothing-much-.git
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git push -u origin branch
The authenticity of host 'github.com (20.207.73.82)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? y
Please type 'yes', 'no' or the fingerprint: yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
Enumerating objects: 25, done.
Counting objects: 100% (25/25), done.
Delta compression using up to 4 threads
Compressing objects: 100% (24/24), done.
Writing objects: 100% (25/25), 5.64 KiB | 360.00 KiB/s, done.
Total 25 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
To github.com:parthbagda211/nothing-much-.git
 * [new branch]      branch -> branch
Branch 'branch' set up to track remote branch 'branch' from 'origin'.
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git checkout -b new-feature
Switched to a new branch 'new-feature'
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch -a
  branch
* new-feature
  remotes/origin/branch
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git checkout branch 
Switched to branch 'branch'
Your branch is up to date with 'origin/branch'.
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git merge main
merge: main - not something we can merge
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ ls
admin.py     migrations   repository.py       tests            test_views.py
apps.py      models.py    service.py          test_service.py  views.py
__init__.py  __pycache__  test_repository.py  tests.py
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git status
On branch branch
Your branch is up to date with 'origin/branch'.

nothing to commit, working tree clean
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git checkout new-feature
Switched to branch 'new-feature'
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git add py-codes
fatal: pathspec 'py-codes' did not match any files
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ cd py-codes
bash: cd: py-codes: No such file or directory
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ cd ..
bagda@bagda-HP-EliteBook-840-G3:~/todoapp$ cd py-codes
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/py-codes$ git add pp.py
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/py-codes$ git status
On branch feature

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   pp.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	../../.bash_history
	../../.bash_logout
	../../.bashrc
	../../.cache/
	../../.config/
	../../.gitconfig
	../../.gnupg/
	../../.java/
	../../.lesshst
	../../.local/
	../../.m2/
	../../.pki/
	../../.profile
	../../.python_history
	../../.ssh/
	../../.sudo_as_admin_successful
	../../.swp
	../../.thunderbird/
	../../.viminfo
	../../Desktop/
	../../Downloads/
	../../IdeaProjects/
	../../codes/
	../../serializers.py
	../../snap/
	../../tests.py
	../../todoapp.zip
	../manage.py
	../settings.py
	../tasks/
	../todoapp/
	../../views.py

bagda@bagda-HP-EliteBook-840-G3:~/todoapp/py-codes$ git push -u origin new-feature
error: src refspec new-feature does not match any
error: failed to push some refs to 'origin'
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/py-codes$ git push -u origin pp.py
error: src refspec pp.py does not match any
error: failed to push some refs to 'origin'
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/py-codes$ git branch -a
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/py-codes$ git branch -all
error: did you mean `--all` (with two dashes)?
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/py-codes$ git branch --all
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/py-codes$ cd ..
bagda@bagda-HP-EliteBook-840-G3:~/todoapp$ cd tasks
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch --all
  branch
* new-feature
  remotes/origin/branch
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git diff
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git diff 
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git add pp.py
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git commit -m 'pp.py file added'
[new-feature d8e9f0e] pp.py file added
 1 file changed, 6 insertions(+)
 create mode 100644 pp.py
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git push -u origin new-feature
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 314 bytes | 314.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'new-feature' on GitHub by visiting:
remote:      https://github.com/parthbagda211/nothing-much-/pull/new/new-feature
remote: 
To github.com:parthbagda211/nothing-much-.git
 * [new branch]      new-feature -> new-feature
Branch 'new-feature' set up to track remote branch 'new-feature' from 'origin'.
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch -d new-feature
error: Cannot delete branch 'new-feature' checked out at '/home/bagda/todoapp/tasks'
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch --all
  branch
* new-feature
  remotes/origin/branch
  remotes/origin/new-feature
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch -d new-feature
error: Cannot delete branch 'new-feature' checked out at '/home/bagda/todoapp/tasks'
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch -d remotes/origin/new-feature
error: branch 'remotes/origin/new-feature' not found.
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git checkout branch
Switched to branch 'branch'
Your branch is up to date with 'origin/branch'.
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch -d new-feature
warning: deleting branch 'new-feature' that has been merged to
         'refs/remotes/origin/new-feature', but not yet merged to HEAD.
Deleted branch new-feature (was d8e9f0e).
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch --all
* branch
  remotes/origin/branch
  remotes/origin/new-feature
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git show d8e9f0e
commit d8e9f0e5601431d17e5388208629b5107cb5941e (origin/new-feature)
Author: parthbagda211 <parth.bagda@practo.com>
Date:   Wed Jun 26 18:29:08 2024 +0530

    pp.py file added

diff --git a/pp.py b/pp.py
new file mode 100644
index 0000000..11fb6a5
--- /dev/null
+++ b/pp.py
@@ -0,0 +1,6 @@
+def add(a,b):
+    return a+b
+    
+    
+def minus(a,b):
+    return abs(a-b)
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git reset HEAD pp.py
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git fetch origin 
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 910 bytes | 910.00 KiB/s, done.
From github.com:parthbagda211/nothing-much-
   b5d2ac1..9ab77c2  branch     -> origin/branch
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git checkout -b recovered-branch origin/new-feature
Branch 'recovered-branch' set up to track remote branch 'new-feature' from 'origin'.
Switched to a new branch 'recovered-branch'
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git branch --all
  branch
* recovered-branch
  remotes/origin/branch
  remotes/origin/new-feature
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git log
commit d8e9f0e5601431d17e5388208629b5107cb5941e (HEAD -> recovered-branch, origin/new-feature)
Author: parthbagda211 <parth.bagda@practo.com>
Date:   Wed Jun 26 18:29:08 2024 +0530

    pp.py file added

commit b5d2ac1b52b54c14721f6f020903172485bfc713 (branch)
Author: parthbagda211 <parth.bagda@practo.com>
Date:   Wed Jun 26 18:17:04 2024 +0530

    added all files
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ git clean -df
Removing py-codes/
Removing tests/
bagda@bagda-HP-EliteBook-840-G3:~/todoapp/tasks$ 

