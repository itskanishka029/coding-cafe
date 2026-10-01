
The hidden entries .git, .venv, and .DS_Store appeared in ls -a but not in ls. Inside the .git directory are Git's internal metadata files, object database, pointers, and configuration settings that track all repository history and changes.
Git is offering to track 4 items (the .DS_Store file, README.md, and the week02/ directory containing two files). Yes, .DS_Store is a hidden system file created automatically by macOS, which I did not manually write.
After creating .gitignore, the hidden .venv/ directory and any untracked files matched by the ignore rules disappeared from my git status output.
.gitignore itself should be committed rather than ignored. Committing it ensures that the project's ignore rules are saved in the repository history and shared with collaborators  when pushed to GitHub.
README.md moved from Untracked files to Changes to be committed. In the three-places model, running git add README.md copied the file from my working directory into the staging area (index), marking it as ready to be included in the next commit.
After committing, Git printed the branch name (main), the short commit hash (053d51e), the commit message, and created file modes. It reported that 6 files changed with 36 insertions(+).
The first seven characters of my commit hash (053d51e) are called a short SHA (or short commit hash). They serve as a unique identifier for that specific snapshot in history, allowing me to easily view, reference, or revert back to that exact commit later.
The four steps of the Git edit-stage-commit loop are:
1.Modify/Create files in the working directory.
2.Check status using git status to see what changed.
3.Stage changes using git add < file > to prepare them for commit.
4.Commit changes using git commit -m "message" to save a snapshot to history.