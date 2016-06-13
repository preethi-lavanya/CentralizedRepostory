1. A central repository is initially created.
2. Everybody that wants to use the central repository creates a clone of that repository using git clone.
   e.g: git clone https://github.com/preethi-lavanya/CentralizedRepostory.git
3. New files are added by individual developers using git add, git commit.
4. After commit, before pushing it is necessary to use git pull --rebase. This commands pulls latest commits from mainline and rebases local commits to occur after the latest changes
in mainline. If there are merge conflicts, git pull rebase asks that the users merge the changes manually, add the changed files, commit and push.
5. It offers 3 options
	i) git rebase --continue. Issue this command after manually fixing the conflicts.
	ii) git rebase --skip. Issue this command to skip rebasing this patch. The changes in the commits will be applied on current branch.
	iii) git rebase --abort. This command removes the pending commits and checksout mainline.

