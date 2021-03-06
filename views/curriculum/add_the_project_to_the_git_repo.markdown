# Add the Project Files to the Git Repo

## Goals

It is time to add all the files to the repo now.

### Step 1

Type this in the terminal

```text
git status
```

`git status` tells you everything git sees as modified, new, or missing.
The first time you run this, you should see a ton of stuff.
The second time you run this, you shouldn't see much of anything.


### Step 2

Type this in the terminal

```text
git add .
```

`git add .` tells git that you want to add the current directory (aka .) and everything under it to the repo.

![](/images/info.png) `git add`

With Git, there are many ways to do the same thing.

* `git add foo.txt` adds a file named `foo.txt`
* `git add .` adds all new files and changed files


### Step 3

Type this in the terminal

```text
git commit -m "Added initial project files"
```

`git commit` tells git to actually do all things you've said you wanted to do.
This is done in two steps so you can group multiple changes together.

`-m` is a option that tells git to add the commit message that follows.

You can see what you've just added to the repository in several ways:

```text
git log
```

will show a log of your commit messages with timestamps. Scroll with `f` and `b` and quit the view with `q`.

```text
git log --stat
```

adds some information about which files you changed in each commit and how many lines you deleted or added.

```text
git log -p
```

shows a log of your previous changes in detail.


## Explanation

By checking your application into git now, you're creating a record of your starting point. Whenever you make a
change during today's workshop, we'll add it to git before moving on. This way, if anything ever breaks, or you make a
change you don't like. You can use git as an all-powerful "undo" technique. But that only works when you remember to
commit early and often!

## Next Step

Go on to [Running Your Application Locally](running_your_application_locally)


