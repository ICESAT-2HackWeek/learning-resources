# Getting started on a tutorial

Instructions for getting a tutorial started on Pangeo (in your browser) and saving changes to your copy of a tutorial.

## Start Pangeo in your browser

#### Step 1
Navigate to the [Pangeo JupyterHub for ICESat-2 Hackweek 2020](http://icesat-2.hackweek.io/).

#### Step 2
Sign in using your GitHub account, if you are not already signed in. (First time only: Grant the ICESat-2 Hackweek Organization permissions - this grants you access to the Pangeo computing environment for the Hackweek.)

#### Step 3
Start the Pangeo computing environement. It may take a few moments to start up.


## Get a local copy of the tutorial and follow along
This basic workflow allows you to follow along with tutorials and save changes to your fork while staying up-to-date with any changes made to the master tutorial.

#### Step 1
Navigate to the tutorial repository on [GitHub](https://github.com/ICESAT-2HackWeek).

Fork the tutorial repository to your personal GitHub account via the GitHub web user interface.

For example, https://github.com/friedrichknuth/geospatial-analysis 
forked from https://github.com/ICESAT-2HackWeek/geospatial-analysis .

#### Step 2
Clone the forked tutorial to your machine/Pangeo environment. You can easily copy the link to a repository by selecting the green "clone or download" dropdown and hitting the clipboard icon, which will automatically copy the link for you.

Open a terminal (using the "plus" sign in your Pangeo JupyterHub) and execute:
```
$ git clone https://github.com/friedrichknuth/geospatial-analysis.git
$ cd geospatial-analysis  
```

#### Step 3
Add the upstream master (a link to the tutorial repository you forked) so we can stay up to date with any changes made to the main tutorial.

```
$ git remote add upstream https://github.com/ICESAT-2HackWeek/geospatial-analysis.git
```

#### Step 4
Fetch and merge the latest changes from upstream master.

```
$ git fetch upstream
$ git merge upstream/master
```

#### Step 5
Checkout a branch to make changes and follow along with the tutorial.

```
$ git checkout -b branch_name  
```

#### Step 6
Follow along with the tutorial. You are welcome to make changes and notes as you go, and these will be saved to your forked copy in the next step.

#### Step 7
Commit your changes and push them up to your fork, under your branch.

```
$ git commit -am "A short commit message noting what you have changed here"  
$ git push origin branch_name  
```

Now your fork will have your changes backed up to GitHub under your branch.

If additional changes were made to the upstream master tutorial, you can checkout the master branch `$ git checkout master` and repeat step 4 to get the latest content, then checkout a new branch with a different name and follow along from there.

*** Please note: the Pangeo JupyterHub you are using for this Hackweek should not be relied upon to save your changes, and will be removed a few weeks after the Hackweek. Thus, you MUST complete Step 7 to push the changes to your GitHub fork of the tutorial if you would like to have continued access to any tutorial notes or changes you made. ***


----
Adapted from https://github.com/ICESAT-2HackWeek/topohack/wiki/Git-workflow-for-tutorials
Originally from https://medium.com/sweetmeat/how-to-keep-a-downstream-git-repository-current-with-upstream-repository-changes-10b76fad6d97
