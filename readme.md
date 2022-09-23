# Git
![Git](https://upload.wikimedia.org/wikipedia/commons/e/e0/Git-logo.svg)
## Introduction:
## Definition
- Git is a distributed open-source version control system (VCS)
- Applications:
  - Solo Project
  - Class project
  - Overcome Your Fear Boot Camp projects
  - Workplace
## Installation - One-off
- Git is free and easy to install on Linux, Windows and MacOS.
- [Link to use to install](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Configuration - One-off
We need to configure git so it identifies us when we create our versions, and when we push them to remote repositories.
- git config --global user.name "Peter Mutisya"
- git config --global user.email info@pmutisya.com

### Initialize Repository
> What is a repository?
> Refers to a 'project' in git. It tracks the versions of all changes made.  It also keeps metadata.
> This info goes into a .git folder in the repository folder.
> Local Repository: Exists on your laptop
> Remote repository: Exists on a VCS server like Github, Bitbucket, Gitlab.
To initialize a local repository:
> git init
To initialize a remote repository, you can use ui controls.

## Working areas in git
- Staging: Files that are tracked, that is they will be part of the next version.
- Unstaged changes: These are changed on the working directory which are not yet staged.
- 

## Working with Git - Day-to-day
- To get a remote repository to your local machine, run: `git clone <url> <destination folder - Optional>`
- `git status`: Gives you information about your current branch. A branch is a line of development.
- `git add <file or folder>`: To include the file(s) into the staging area.
- `git commit`: To add staged changes to a version. This serves as a checkpoint in our project which we can always come back to.
- `git log`: To see history of commits/versions.
- `git checkout <commit hash>`: To go back to a certain commit.
- `git revert`: Go back to the past commit.

## Interacting with remote repository
- `git pull`: get and apply updates from remote repository. This is actually two commands in one.
  - `git fetch`: Get updates from remote repo
  - `git merge`: Apply changes to the local repository.

## Branches
![Branching](https://wac-cdn.atlassian.com/dam/jcr:389059a7-214c-46a3-bc52-7781b4730301/hero.svg?cdnVersion=542)
- A branch is a line of development.
- `git branch` or `git branch --list`: : Show current branch
- `git branch branch-name`: Create branch named branch-name
- `git branch -d existing-branch`: Delete existing-branch
- `git merge destination-branch`: integrates or applies changes from the current branch to destination-branch.

## Pull Requests, Review and Conflicts
- A pull request is a feature of many remote VCS solutions. It allows you to tell others what that you have made some changes, and they can see the changes made. Discussions can follow up.
- Once the users are satisfied with your changes, they can allow you to merge the branch (accept your changes into the team's branch).
- You are encouraged to take the review process seriously.
- Conflicts ensure where there is a clash of versions. E.g your changes and the changes of your team mate collide. There are 3 ways to resolve a conflict.
1. Pick the first person's changes and ignore the second's.
2. Pick the second person's changes only and ignore the first's.
3. Create a new change which is a combination of both. This is the preferred approach, and is commonly done as a manual process.

How to avoid conflicts.
It's worth noting that conflicts waste a lot of time, and can bring a lot of errors to a project. Features can be lost midway. To avoid conflicts:
1. Share work well in such a way that multiple people are not working on the same files.
2. In case you are working on the same file, do so with small commits, pushes and pulls. This reduces chance of conflicting.


## Branching Policy
![Branches](https://wac-cdn.atlassian.com/dam/jcr:c6db91c1-1343-4d45-8c93-bdba910b9506/02%20Branch-1%20kopiera.png?cdnVersion=542)

- How do we create our branches and how do we name them?
- Branch names need to be descriptive of what is supposed to be done. E.g adding-api-users
- Git repositories are created with a default branch. This branch is commonly called `master` or `main`.
- Some developers also create a new branch commonly called `develop` which is the destination branch for development work.
- branches can also be prefixed to explain the nature of the task in question. This makes your branch intuitive. The most common branch prefixes used include:
- feature: e.g `feature/create-users`
- bugfix: e.g `bugfix/users-not-able-to-log-in`
- hotfix: Refers to deliver a quick fix in production. e.g `hotfix/kafka-failing`
- release: Refers to a version delivered to the users. e.g `release/5.7.2`

A good branching policy helps improve issue traceability and prevents conflicts.



# Bonus
## Issues
- Most of the software planning is done outside the branches. For this,w e use issue tracking solutions such as Jira, Bitbucket issues and Github issues.
- Here is where discussions happen.
## Commit Messages
- When messaging your commits, please use descriptive names. A commit message should explain what you've done, not what you expected to do or what you wanted to achieve. Be direct.
- Also, consider using multiline messages.

## Credential cache
This stores your credentials in memory when you're working so you don't have to keep typing your credentials.
- git config credential.helper <options>
- git config credential.helper cache --timeout <seconds>

## Stashing
- Keep your changes save until you need them
- `git stash`: To save changes in a local store
- `git stash pop`: To get back saved changes. 
- Remember this is a stack (pop). So if you do stash1, then stash2, then stash3, pop1 will give you stash 3, pop 2 stash 2 and pop3 stash 1.
- Also, stashes are not depended in the branch. So you can stash, checkout to another branch, then pop your stash.

## Authentication options
### SSH
> [A link to help you do this](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

### App Password
> https://support.atlassian.com/bitbucket-cloud/docs/app-passwords/


## Markdown
- A simple, yet very powerful markup language. You can use it to add format to plaintext.
- You will be needed to use it to write your Readme.md file.

## Git Ops
- This is a way of implementing CI/CD. It incorporates VCS, collaboration and compliance to service automation.

## More resources
Truth be told, there is more to git. We've just talked about what you need for dy-to-day operations.
- https://www.atlassian.com/git/tutorials/using-branches/git-merge
- https://dev.to/valeriavg/master-git-in-7-minutes-gai