# my git config #

## aliases ##

Alias | Description
--- | ---
git s | Show current branch and ahead/behind status
git f | Fetch remote repository 'origin'
git b | Show local branches
git br | Show remote branches
git st  | Stage all changes
git un  | Unstage all changes
git m Fixed button | Create a commit with given message (no quotation marks needed!)
git mj Fixed button | The same, but with prefix like 'ASD-335: '
git head | Show current branch name
git prev | Show previous branch name 
git rel |  Show last local and remote release branches (project-specific)
git c john/ASD-321 | Checkout existing local branch
git co john/ASD-475 | Checkout remote branch from origin
git cn  john/ASD-557 | Create and checkout new branch
git cr | Checkout last local release branch (project-specific)
git crr | Checkout last remote release branch (project-specific)
git cp | Checkout previous branch
git cd | Fast-forward and checkout 'develop' branch
git cm | Fast-forward and checkout 'master' branch
git ct | Checkout 'temp' branch here
git ch 355c3ad | Cherry-pick commit 355c3ad
git chc | Cherry-pick continue
git cha | Cherry-pick abort
git ph | Push head (create new branch on remote)
git pf | Push force
git db | Delete current branch with switching to 'master'
git dbf | The same, but force
git dr | Delete remote branch (upstream) for current branch
git du | Show only unstaged changes (diff between working copy and staging)
git ds | Show only staged changes (diff between staging and head)
git da | Show all uncommited changes (diff between working copy and head)
git df | Show file change statistics
git amn | Amend last commit from staging
git amm | The same but with message editing
git mu | Merge upstream, no fast-forward
git mp | Merge previous branch, no fast-forward
git md | Merge 'origin/develop'
git mm | Merge 'origin/master'
git mt | Merge 'temp' branch
git mc | Merge continue
git ma | Merge abort
git ru | Rebase on upstream
git rp | Rebase on previous branch
git rd | Rebase on origin/develop
git rdt | Rebase on origin/develop automatically resolving conflicts with 'theirs' <br> (taking our changes from current branch)
git rc | Rebase continue
git ra | Rebase abort
git ri e9b838e | Start interactive rebase
git ff | Fast-forward current branch to upstream
git fff | Fetch and fast-forward to upstream
git ffd | Fast-forward 'develop' (without checkout)
git ffm | Fast-forward 'master' (without checkout)
git noff john/ASD-335 |  Merge 'john/ASD-335', no fast-forward
git temp | Create 'TEMP commit' from all uncommited changes
git soft | Disassemble last commit into staging (typically to reverse 'git temp')
git hardu | Do a hard reset of current branch to upstream
git me | Show my username and email
git or | Show 'origin' remote repository url
git rem | Show all remote repositories
git v | Show git version
git cat d2f54a0 | Show commit metadata
git time | Show date '2018-09-28_12-04-41' (used in 'git back')
git udfh | Discard any changes in file 'SQL/UDF.xml' during merge conflict (project-specific)
git udfd | Reset file 'SQL/UDF.xml' to 'origin/develop' state (project-specific)
git lp | Log with pretty format
git l  | Show last commit
git l1 | Show last 10 commits
git l2 | Show last 11-20 commits
git l3 | Show last 21-30 commits
git l4 | Show last 31-40 commits
git l5 | Show last 41-50 commits
git lu | Show new remote commits from upstream (behind)
git ll | Show new local commits yet to be pushed (ahead)
git lf *tsconfig.json | Show all commits affecting file 'tsconfig.json'
git la Alex |  Show all commits authored by 'Alex'
git lm 'one more' | Show all commits with message 'one more'
git lw | Show all my commits since last week
git back | Create backup branch (without checking it out) 'my-branch-backup/2018-09-28_12-07-55'
git copy 8e92d6b | Make current branch exact as given commit by adding new commit 'Tree copy from 8e92d6b'
git com | Compare current branch with 'origin/develop'
git com john/alpha | Compare current branch with 'john/alpha'
git com john/alpha origin/john/beta | Compare 'john/alpha' with 'origin/john/beta'
git com a17dd93 165db4a | Compare two given commits
git rvm | Start 'rebase via merge' script
git debug lm 'one more' | Show tracing info for given git command
git con | Edit local config file
git cong | Edit global config file
git al | Show all aliases


## alias combos ##

Commands | Description
--- | ---
git f <br> git ct <br> git md <br> #resolve&nbsp;conflicts <br> git mc <br> git cp <br> git rdt <br> git copy temp <br> git amm | Perform rebase of current branch on 'origin/develop' dealing only with final merge conflicts. This method is a less pain alternative to classic rebase when you have conflicts on multiple commits.
git rvm | The same but with script
git cd <br> git mp | Merge current branch into 'develop'


## config location ##

Type | Location
--- | ---
Repository-specific (local) | my-project/.git/config
Edit local config file | git config --local --edit
Show user-global location | echo $HOME
User-global on Linux, Mac | ~/.gitconfig
User-global on Windows | C:\Users\UserName\\.gitconfig
The same | %UserProfile%\\.gitconfig
Edit global config file | git config --global --edit
