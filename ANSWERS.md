# Assignment 2 – College Fest Website

**Q1: Which of your merges was a fast-forward and which were 3-way? How could you tell from Git's output and from the graph?**

**Ans:** The merge of feature/schedule into main was a fast-forward merge. Git displayed the message "Fast-forward", and the commit graph showed a straight line without a separate merge commit.
The merges of feature/registration and feature/sponsors into main were three-way merges. Git created separate merge commits using the ort strategy, and the commit graph showed branches joining together.

**Q2: What does HEAD point to normally, and what changed in Step 7? Why is it risky to make commits in a detached HEAD state?**

**Ans:** Normally, HEAD points to the current branch, which points to the latest commit. In Step 7, HEAD pointed directly to an older commit instead of a branch. This is called detached HEAD state. Making commits in this state is risky because they are not automatically attached to a branch and may become difficult to find later.

**Q3: Why did git branch -d refuse to delete experiment/dark-theme? When would git branch -D be the wrong choice?**

**Ans:** Git refused to delete experiment/dark-theme because its commit had not been merged into main. The -D option forcefully deletes a branch even if it contains unmerged work. Using -D would be the wrong choice when the branch contains important changes that have not been merged or backed up.

**Q4: git switch and git checkout can both change branches. Why was git switch introduced, and what else can checkout do?**

**Ans:** Git switch was introduced to provide a simpler and more specific command for switching and creating branches. Git checkout can also switch branches, but it can do more than that. It can restore files and move HEAD to an older commit, which can result in a detached HEAD state.

**Q5: A teammate always commits straight to main. Explain in 3–4 sentences why feature branches are a safer workflow for the fest team.**

**Ans:** Feature branches allow each team member to work on separate features without directly changing the main branch. They reduce conflicts and prevent unfinished code from affecting the main website. Changes can be tested and reviewed before merging. This makes teamwork safer and keeps the project organized.