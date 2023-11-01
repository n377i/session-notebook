# Git Workflow

## Initialising Git Repository

Located in the folder we want to work in:

```
git init
```

Will reply like:

```
Initialized empty Git repository in {...}/my-website/.git/
```

## See project status

```
git status
```

Response:

```
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.md
	index.html
	style.css

nothing added to commit but untracked files present (use "git add" to track)
```

## Preparing the commit: staging

We invite the files we need to the picture like:

```
git add index.html
git add styles.css
```

A `git status` shows:

```
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   index.html
	new file:   style.css

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.md
```

## Taking the actual picture: commit

```
git commit -m 'First version of the homepage.'
```

Success feedback:

```
[main (root-commit) d1e4dd5] First version of the homepage.
 2 files changed, 87 insertions(+)
 create mode 100644 index.html
 create mode 100644 style.css
```

After that, `git status`:

```
d1e4dd5 (HEAD -> main) First version of the homepage.
```

## Tl;DR

```
git add .
git commit -m 'Some work'
git push
```
