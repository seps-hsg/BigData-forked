# Big Data Statistics for R and Python

## Course materials for Part I

- See `materials/slides` for the weekly lecture slides.
- See `materials/notes` for the weekly lecture notes.
- See `materials/sourcecode` for the code examples shown in the notes.


## Work with Git/GitHub

*NOTE:* Depending on your operating system, you might have to install Git manually before using it with RStudio. You will find detailed instructions [here](https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN).

## Clone this course's repository

1. In RStudio, navigate to a folder on your hard-disk where you want to have a local copy of this course's GitHub repository.
2. In RStudio, switch to the Terminal, and type the following command.

```
git clone https://github.com/umatter/BigData.git
```

This creates a new directory `BigData` with all the course material in it.
Whenever there are some updates to the course's repository on GitHub, you can update your local copy with:
```
git pull
```
(Make sure you are in the `BigData` folder when running `git pull`.)


## Fork this course's repository

1. Go to [`https://github.com/umatter/BigData`](https://github.com/umatter/BigData), click on the 'Fork' button in the upper-right corner (follow the instructions).

2. Clone the forked repository (see the cloning of a repository above for details). Assuming you called your forked repository `BigData-forked`, you run the following command in the terminal (replacing `<yourgithubusername>`:

```
git clone https://github.com/`<yourgithubusername>`/BigData-forked.git
```

3. Switch into the newly created directory:

```
cd BigData-forked
```

4. Set a remote connection to the *original* repository

```
git remote add upstream https://github.com/umatter/BigData.git
```

You can verify the remotes of your local clone of your forked repository as follows
```
git remote -v
```
You should see something like
```
origin	https://github.com/<yourgithubusername>/BigData-forked.git (fetch)
origin	https://github.com/<yourgithubusername>/BigData-forked.git (push)
upstream	https://github.com/umatter/BigData.git (fetch)
upstream	https://github.com/umatter/BigData.git (push)
```

5. Fetch changes from the original repository. New material has been added to the original course repository and you want to merge it with your forked repository. In order to do so, you first fetch the changes from the original repository:

```
git fetch upstream
```

6. Make sure you are on the master branch of your local repository:

```
git checkout master
```

7. Merge the changes fetched from the original repo with the master of your (local clone of the) forked repo.

```
git merge upstream/master
```

8. Push the changes to your forked repository on GitHub.

```
git push
```

Now your forked repo on GitHub also contains the commits (changes) in the original repository.

# HELLO WORLD
