INTRODUCTION:

Git is a distributed system, no notion of primary server or master server. 
Its a distributed system, each copy of repository is independent copy. 
Essentially we need to so locally.
We should talk to peer to peer relationship 

GITHUB
Its a software as a service very popular, hosting online git repository.
GITHUB is a SaaS, which use git under the hood. 
Its been a central server, more of workflow basics as suppose to be inherit

What is the meaning of Repository ?

Set of information, that stored in the GIT folder.
Git by default make a specifi view into the file. View of these specific files in notion of branches. 
By default Git make it as a branch as Git Master.


How to create a Git Repository :

Step 1 : git init (Which will initilize). 
Step 2 : git status (To look at the status of the repository) 
         Git Status tell us that we are in the git master and commit details
Step 3:  Create files. And when you check the "git status", you will find On the branch Master, we do not have any commit
         The newly created files are not tracked. 
Step 4:  Now we need to add the file "git add ." Once we have "git add ." we notice that the changes to be committed.
         In this they moved into the staging state. 

Note : Git has three stage process, first we need to add or remove in the staging area, basically make a snapshot 

Step 5:  git commit -m "<COMMENT>" this comment will be associated with this commit. 

Note : Before you commit, at first time we need to set the email address and username. It will store this locally in the configfile. 

git config --global user.email "you@email.address"
git config --global user.name "yourname"

Bascially it stores this in ~/.gitconfig

How Git Works ?

Git has three different views. 

Actual Repository : What stores in the actual .git folder. Check using "cd .git/". Check using tree.
Working Directory : We have all the commited file in the Working Directory. 
Staging : Add and remove between the working directory and staging takes place. 

[saby@saby git-test]$ cd .git/
[saby@saby .git]$ tree
.
├── branches
├── COMMIT_EDITMSG
├── config
├── description
├── HEAD
├── hooks
│   ├── applypatch-msg.sample
│   ├── commit-msg.sample
│   ├── fsmonitor-watchman.sample
│   ├── post-update.sample
│   ├── pre-applypatch.sample
│   ├── pre-commit.sample
│   ├── prepare-commit-msg.sample
│   ├── pre-push.sample
│   ├── pre-rebase.sample
│   ├── pre-receive.sample
│   └── update.sample
├── index
├── info
│   └── exclude
├── logs
│   ├── HEAD
│   └── refs
│       └── heads
│           └── master
├── objects
│   ├── 20
│   │   └── 22944635d9d194891c34b8e378e604e49b6611
│   ├── 52
│   │   └── 7c4c2283154379ded3d592612ae509a2f55e72
│   ├── ac
│   │   └── 55a86c931fd1861d8a64d3bea1c33f5f170963
│   ├── info
│   └── pack
└── refs
    ├── heads
    │   └── master
    └── tags


Issue the command "git branch"

"git diff" to check what are the changes done. 

"git log" Its will show us the history of commits. Note the bottom one will always be the first commit. Then move on
On each commits we make the snapshot of the files. 

  Some more addition required
