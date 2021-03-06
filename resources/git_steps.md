## Git Steps

### Overview

<p align="center">
  <img src="images/overview.jpg">
</p>

### First time only

1. In GitHub, fork the repository, https://github.com/uvastatlab/statlab-fellows, to your own github account and go to the forked repository; click on "Clone or Download" and copy the repository URL to the clipboard.

2. In the terminal, navigate to your local directory (where you want the repository to live)

```sh
$ cd "box sync/mpc/datafordemocracy/" # this will be different for you
```

3. Clone the repository locally

```sh
$ git clone https://github.com/mclaibourn/statlab-fellows.git # use your GitHub name/url
```

4. Navigate to the new repository

```sh
$ cd statlab-fellows
```

5. Tell git about the source repository [(more here)](https://help.github.com/articles/configuring-a-remote-for-a-fork/)

```sh
$ git remote -v # initially only your forked repository should be listed
$ git remote add upstream https://github.com/uvastatlaby/statlab-fellows.git # "upstream" is a name we provided to reference the source repository
$ git remote -v # verify
```

### Syncing local files with source repository

Before adding changes from the repository on your local machine to the forked repository on GitHub (the one in your account,
[see more here](https://help.github.com/articles/syncing-a-fork/), make sure you're working with the most recent files.

1. In the terminal, navigate to your local directory

2. Fetch the contents of the source repository, fellows. so you're starting with the most recent version

```sh
$ git fetch upstream
```

3. Merge the changes from upstream/master into your local master branch

```sh
$ git merge upstream/master # this brings your fork's master branch (working directory) in sync with the source repository's master branch)
```

4. Your local copy of the repository is updated; now update your fork on GitHub

```sh
$ git push origin master # pushes the name on your local machine (origin) to a branch on your GitHub page (master)
```

### Working with/changing files in the forked GitHub repositry

For some files, e.g, markdown/text files like the weekly updates, it's simpler to make the changes within GitHub.

1. Click edit button on the file page; make changes
2. Click "commit changes" button -- GitHub will provide a default title, but you can change this and add description if you like
3. Create a pull request following steps 1-3 in ["Make a pull request"](#pull) below

Once the pull request has been merged GitHub will send you a notification. You should sync the source repo with your local repo (on your computer) following the steps 1-3 above to ensure your changes are reflected in all three locations.


### Working with/changing files on your local repo (on your computer)

In most cases, e.g., making changes to code, you'll make changes on your local machine first. When you're ready, commit those changes to your local repository, push these to your forked repository on GitHub, and create pull request to merge them into the source repository.

1. Once you're satisfied with changes, open the terminal/bash and navigate to your local directory

2. List new or modified files available to be committed

```sh
$ git status
$ git diff # show file differences; use q to exit results
```

3. Stage files for commit, then commit 

```sh
$ git add [file]
$ git commit -m "[add commit message]"
```

You can use --all to commit all changes at once if there are multiple changes.

4. Push these changes to your forked repo

```sh
$ git push origin master
```
5. Then create a pull request following steps 1-3 in ["Make a pull request"](#pull) below.


### Syncing local files with source repository (alternative method)

In this method, we'll be using ```git pull``` to sync changes with the remote repository and make use of branch to avoid
merge conflicts.

Before adding changes from the repository on your local machine to the forked repository on GitHub (the one in your account, [see more here](https://help.github.com/articles/syncing-a-fork/), make sure you're working with the most recent files.

1. Have a branch for development
```sh
$ git branch dev  # This will create a branch called dev
$ git checkout dev # This will switch to the branch called dev instead of master

```
2. Now that you have a branch, edit your files in your branch (whatever code changes you want to make) and stage it

```sh
$ git add 'files you edited and you want to include'
$ git commit -m <insert commit message>
```

3. Working with pull

Now you have your changes in the local branch called dev. You need to find a way to sync our local repository to
upstream. In order to do this and avoid merge conflicts, you need to sync your local master with remote (upstream) and merge your changes (on branch dev)
on top of it

```sh
$ git checkout master # switch to branch master
$ git pull upstream master # Pull all changes to branch master
```
At this point, your repository looks something like this:

<p align="center">
  <img src="images/branch.jpg">
</p>

You need to merge your changes with the local master and push it to the forked repo. In order to do that, use the
following code

```sh
$ git merge dev    # git will prompt you with a commit file, this is fine. Save it.
$ git add <Files you need to push>
$ git commit -m "Your new commit name"
$ git push origin master  # This will push changes to the forked repository
```

<a name="pull"></a>
### Make a pull request
When you want to add the changes from your forked repository on GitHub to the source repository

1. From the forked repository on your GitHub click "New pull request" (this will send you to the source repository)

2. In "compare across forks", the base fork is the original source repository, the head fork is your fork

3. Give your request a title and description and click "Create pull request"


## Some useful links

* [syncing your local to remote](https://www.atlassian.com/git/tutorials/syncing)
* [cheatsheet for Git](http://supercollider.github.io/development/git-cheat-sheet)
* [Git interactive tutorials](https://try.github.io/levels/1/challenges/1)
* [Learn git branching](http://learngitbranching.js.org/)

