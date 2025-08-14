### GIT:

- [Download Link](https://git-scm.com/download/win)
- Install using default settings

#### Use:

- Using `CMD` or `PowerShell` (would recommend using `PowerShell` for quality of life features like using `Ctrl` + `Spacebar` to get suggestions when trying for example to `cd`)
- Typing `git` and hitting `Enter` should (if installed correctly) give short list of possible commands

#### Commands:

- `git config --global user.name "<Your Name>"`
- `git config --global user.email "<yourname@example.com>"`
- `git config --global init.defaultBranch main` -> default branch name changed from `master` to `main`
- `git config --global color.ui auto` -> enable colorful output with `Git`
- `git config --global pull.rebase false` -> default branch reconciliation behavior to merging
- `git config --global http.proxy http://user:password@host:port` -> to setup `Git` to use proxy
- `git config --list` -> check if config set properly
- `git config --global --unset <configname>` -> unset config option
- `git init` -> initalizes a new `Git` repository in the current directory
- `git add <filename>` -> adds file to the stage; tells `Git` which files to include in the next commit; Using `.` instead of `<filename>` will add all files and subdirectories in directory where `Git` was initalized
- `git commit -m "<message>"` -> saves changes to repository, it is like a snapshot of your project at a specific point of time allowing you to revert changes to the codebase if needed; Replace `<message>` with comment that will describe changes made in the current stage
- `git remote add origin <link>` -> adding remote origin
- `git remote remove origin` -> remove remote origin
- `git branch -M main` -> rename main/master branch
- `git push -u origin` -> push local `Git` commits to a remote repository
- `git clone <url>` -> clone remote repository to local directory
- `git clone -b <branch-name> <url>` -> clone specific branch
- `git status` -> displays current status of the repository
- `git log` -> displays commit history if a `Git` repo
- `git branch -d <branch name>` -> delete branch from local repo
- `git push origin --delete <branch name>` -> delete branch from remote repo
- `git merge <branch name>` -> merge current branch with the branch of <branch_name>
- `git checkout -b <branch name>` -> create new local branch and switch to it
- `git rm --cached <filename>` -> remove cached file from tracking if added later to .gitignore or file renamed and should not be tracked
- `git branch -D <branch name>` -> delete branch without merging it
- `git checkout <branch name>` -> change working branch to <branch_name>
- `git branch --all` -> pull all branches including remote ones that are not downloaded locally
- `git pull origin <branch name>` -> pull branch of name to current branch
- `git fetch --all` -> fetches all branches
- `git fetch origin` -> Fetch all new branches and commits from the remote
- `git reset --hard origin/<branch_name>`-> discard all local changes and commits, aligning the branch with its remote
- `sudo -E git <command/s>` -> preserves user env config when running as sudo
- `git -c user.name="Your Name" -c user.email="your@email.com" commit -m "Your commit message"` -> oneliner commit wihtout specyfing global user.name and user.email
- `git restore .` -> restore all unstaged files in current directory
- `git restore path/to/file/to/revert` -> restore specific file
