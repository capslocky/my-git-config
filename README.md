# my git config #

## aliases ##

Alias | Description
--- | ---
git s | Show current branch and ahead/behind status
git f | Fetch remote repository
git b | Show local branches
git st  | Stage all changes
git un  | Unstage all changes
git m Fixed button | Create a commit with given message (no quotation marks needed!)
git head | Show current branch name
git prev | Show previous branch name 
git rel |  Show last local and remote release branches (project-specific)
git c baur/ASD-321 | Checkout existing local branch
git co baur/ASD-335 | Checkout branch from origin
git cr | Checkout last local release branch (project-specific)
git crr | Checkout last remote release branch (project-specific)
git cp | Checkout previous branch
git cb  baur/ASD-342  | Create and checkout new branch
git cd |  Checkout 'develop' branch
git cm | Checkout 'master' branch
git ch 355c3ad | Cherry-pick commit 355c3ad
git ph | Push head (create new branch on remote)
git pf | Push force
git db |  Delete current branch with switching to 'master'
git dbf | The same, but force
git dr | Delete remote branch (upstream)
git am | Amend last commit from staging
git amm | The same but with message editing
git mu |  Merge upstream
git md |  Merge origin/develop
git mc |  Merge continue
git ma | Merge abort
git ru | Rebase on upstream
git rd | Rebase on origin/develop
git rc | Rebase continue
git ra |  Rebase abort
git ff |  Fast-forward to upstream
git fff |  Fetch and fast-forward to upstream
git noff baur/ASD-335 |  Merge 'baur/ASD-335' without fast-forward
git temp |  Create 'TEMP' commit from all uncommited changes
git soft |  Disassemble last commit into staging (typically to reverse 'git temp')
git hardu | Do a hard reset of current branch to upstream
git lp | Log with pretty format
git l  |  Show last commit
git l1 |  Show last 10 commits
git l2 | Show last 11-20 commits
git l3 |  Show last 21-30 commits
git l4 | Show last 31-40 commits
git l5 |  Show last 41-50 commits
git lf *tsconfig.json | Show all commits affecting file 'tsconfig.json'
git la Alex |  Show all commits authored by 'Alex'
git lm 'one more' | Show all commits with message 'one more'
git lu |  Show all new commits in upstream
git com | Compare current branch with 'origin/develop'
git com baur/alpha |  Compare current branch with 'baur/alpha'
git com baur/alpha origin/baur/beta |   Compare 'baur/alpha' with 'origin/baur/beta'
git com a17dd93 165db4a | Compare two given commits
git al | Show all aliases
git debug lm 'one more' | Show tracing info for given git command


## config location ##

Type | Location
--- | ---
Repository-specific | my-project/.git/config
Show user-global location | echo $HOME
User-global on Linux, Mac | ~/.gitconfig
User-global on Windows | C:\Users\UserName\\.gitconfig
The same | %UserProfile%\\.gitconfig
Edit config file | git config --global --edit