# Getting started on a tutorial

These are instructions for getting a tutorial started on Pangeo (in your browser) and updating the tutorial. If you would like to take notes, please do so in an external document or your personal fork of the tutorial repository (if you know what that means).

## Start Pangeo in your browser

#### Step 1
Navigate to the [Pangeo JupyterHub for ICESat-2 Hackweek 2020](http://icesat-2.hackweek.io/).

#### Step 2
Sign in using your GitHub account, if you are not already signed in. (First time only: Grant the ICESat-2 Hackweek Organization permissions - this grants you access to the Pangeo computing environment for the Hackweek.)

#### Step 3
Start the Pangeo computing environement. It may take a few moments to start up.


## Get a local copy of the tutorial and follow along
This basic workflow allows you to follow along with tutorials while staying up-to-date with any changes made to the master tutorial.

#### Step 1
Navigate to the tutorial repository on [GitHub](https://github.com/ICESAT-2HackWeek).

Clone the tutorial to your machine/Pangeo environment. You can easily copy the link to a repository by selecting the green "clone or download" dropdown and hitting the clipboard icon, which will automatically copy the link for you.

Open a terminal (using the "plus" sign in your Pangeo JupyterHub) and execute:
```
$ git clone https://github.com/ICESAT-2HackWeek/geospatial-analysis.git
$ cd geospatial-analysis  
```

_Note: a more detailed version of step 1, including images, is available as part of the [Preliminary Steps - JupyterHub Connection](https://icesat-2hackweek.github.io/learning-resources/preliminary/jupyterhub/#how-do-i-get-my-code-in-and-out-of-pangeo)._

#### Step 2
Add the origin master (a link to the tutorial repository you cloned) so we can stay up to date with any changes made to the main tutorial.

```
$ git remote add origin https://github.com/ICESAT-2HackWeek/geospatial-analysis.git
```

#### Step 3
Update your local copy with any changes to the master copy. If you have tried to save notes or changes within your local copy of the notebook, this may cause conflicts. 
Fetch and merge (using git pull) the latest changes from origin master.

```
$ git pull origin
```

#### Step 4
Follow along with the tutorial. You can save your notes (if you're taking some in the Pangeo text editor) by downloading a copy to your local machine.



If additional changes were made to the origin master tutorial, you can checkout the master branch `$ git checkout master` and repeat step 3 to get the latest content.

*** Please note: the Pangeo JupyterHub you are using for this Hackweek should not be relied upon to save your documents beyond the duration of the Hackweek, and will be removed a few weeks after the Hackweek. Thus, for any non-repository changes or repository changes that have not been pushed to GitHub, you MUST complete Step 4 to save the files to your local machine if you would like continued access to them. ***


----
Adapted from https://github.com/ICESAT-2HackWeek/topohack/wiki/Git-workflow-for-tutorials
Originally from https://medium.com/sweetmeat/how-to-keep-a-downstream-git-repository-current-with-upstream-repository-changes-10b76fad6d97
