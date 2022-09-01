<b>GIT GUIDE</b>

<b>FIRST TIME CONNECTING TO GITHUB REPO</b>
* Make a GitHub account
* Go to https://github.com/osheets/LT4_SakayDB 
* Click fork (top right)
* Wait until ready
<b>New Terminal in Jupyter Notebook</b>
* Mkdir myrepo
* Cd myrepo
* Git init
* Git config --global init.defaultBranch main
* Git config --global user.name “Firstname Lastname”
* Git config --global user.email  “validemail@gmail.com”
* Git config --global core.editor “vim”
* Git branch
* If name is not “main”
    * Git branch -M main
* Git clone https://github.com/<YOUR-USERNAME>/LT4_SakayDB.git
* Cd LT4_SakayDB
<b>MAKING YOUR BRANCH</b>
* Git branch <your-branch>
* Git branch (to see all branches, and current branch)
<b>SWITCH TO THAT BRANCH</b>
* Git checkout <your-branch>


<b>ADD CHANGES</b>
1. CHECK IF IN RIGHT DIRECTORY and BRANCH
* Cd myrepo/LT4_SakayDB
* Git checkout <your-branch>
2. ADD (staging)
* Git add <file to be added>
* or if deleting, Git rm <file to be deleted>
* Git status (text should be red and ready)
3. COMMIT (committing locally)
* gitGit commit -m “Description of what you revised”
* Git status (text should be all green)
4. PUSH (pushing to GitHub)
* Git push -u origin <your-branch> (if first time on a branch)
    * Or git push origin <your-branch>

<b>CHECK CHANGES</b>
* Git log (make sure youre on the branch you want to see the history of)
* Git diff <branch1> <branch2> (diffs between branches)
* Git diff <code of commit 1> <code of commit 2>
* Git diff HEAD~1 (difference between most recent commit)

<b>SYNC WITH GITHUB VERSION</b>
* Git checkout main
* Git pull origin


——[don’t try this yet vvv]——

SYNC USING PULL REQUEST…
* Git remote -v (should see your fetch and push link)
* Git remote add upstream https://github.com/osheets/LT4_SakayDB.git
* Git remote -v (should see your username - origin, osheets - upstream)
—
* Git checkout main
* Git merge upstream/main
— Go to your forked repo
* New pull request

