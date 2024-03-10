# Git Commands
- **Git clone from Branch:**
  - git clone -b release/v1.1.0 'clone_url'
- **Get new updated files from git**
  - git checkout --all
  - git checkout .
  - git checkout branchname
  - git pull origin 'branch name'
  - git pull 'branch name'
  - git pull .
  - git fetch
  - git pull .
- **Create new branch**
  - git checkout -b feature/PVCAID-20505-Design-PVCAID-18145
- **Add changes:**
  - git add .
  - git commit -m 'comment'
  - git push branch origin 'branch-name'
  - git commit 
- **Merge branch:**
  - git checkout 'Parent branch'
  - git pull origin 'Parent Branch'
  - git merge 'child branch'
  - git push 
- **Discard local changes and pull files:**
  - git reset --hard
  - git pull
- **Discard local changes**
  - $ git restore .
- **Restore and remove complete folder without retart**
  - Note: Reset git before checking new branch

  - git reset –hard  (remove all changes from all env, brings the original copy)
  - git clean -fxd
    
- **Deleting a file**
  - git rm add.txt --> removing manually + git add .
  - 
- **Discard changes before commit:**
  - git reset

- **Submodule commands:**
  - git submodule add "submodule path" shared-param

  - git submodule init
  - git submodule sync
  - git submodule update --init --remote
  - git submodule update --remote
  - /.file.sh d4r1

- **pre-commit:**
  - git add .
  - pre-commit run
    OR
  - pre-commit run --all-files


- **Undo single file (To make it to its orginial form):**
  - git checkout -- filename

- **Go check current branch name:**
  - git branch --show-current

- **PR Commit messages:**
  - New feature commit - git commit -m 'feat: storyPVCAID-message' (Will increase a version)
  - Bug fix commit - git commit -m 'fix: bugPVCAID-message' (Will increase a version)
  - Comment - git commit -m 'comment: bugPVCAID-message' (Will not increase a version)
  - Test - git commit -m 'test: bugPVCAID-message' (Will not increase a version)


 #=================================
Principles for any git repository

1) Use version control
2) Use tests
3) Have good documentation.
4) Use good structure
5) Keep root clean
	README
	LICENSE
	requirements.txt (or pipfile)
	tests/
	doc/
	your_project_name
	Makefile
	manage.py (Django)
	.yml
	.gitignore


6) Things to avaoid
	Circular dependencies
	Hidden coupling
	Global state/context
	Spaghetti
	Ravioli
