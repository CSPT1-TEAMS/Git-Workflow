# Git Workflow CSPT1 Teams

## Steps to Follow:

1. Go to your terminal and navigate to the directory where you keep all your Lambda School assignments

2. git clone https://github.com/CSPT1-TEAMS/ *current_sprint*

3. **The following is for only one member of the pair (maybe whoever is going to drive first)**
  * Create a branch using the following naming 
    * `git checkout -b team-(my team))_(my-name)-and-(pair’s-name)`*
  * `yarn install` (each person may as well do this)
    * __both people should also follow the setup as described in the readme file as well__
  * then `git push origin <your branch-name>`
  * begin to work on the sprint with your pair as you normally would 
  * __remember to commit often!!__
5. When you want to switch roles 
  * the driver should make any final commits
  * and be sure to `git push origin <your_branch_name>` and __NOT__ `master`

> *An example pair branch would look like "team-b_greg-and-wesley"

## Switching between Driver/Navigator

1. After the original driver has made the final push to the pair branch, the new driver should just need to type the following commands in the directory where the current sprint is located
  * `git checkout <team_branch_name>`
  * `git pull origin <team_branch_name>`

2. This will check out the new driver into the team branch followed immediately by updating (or _pulling_) the code from Github.

#### And when driver/navigator switch up again, just follow the same steps above.

## If the `master` branch is updated

1. Commit all your files
2. Then run the following commands in your terminal
  * `git checkout master`
  * `git pull origin master`
  * `git checkout <your_branch>`
  * `git merge <your_branch> master`

Soon, we will cover more branching along with submitting a pull request into the _dev_ branch of the team repository.

Here are some resources that cover some of these ideas:
* [Excellent Stack Overflow Post](https://stackoverflow.com/questions/2428722/git-branch-strategy-for-small-dev-team)
* [Pro Git](https://git-scm.com/book/en/v2) online book about everything you'd ever want to know about git.
  * And a chapter specifically about [Branching](https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows)
