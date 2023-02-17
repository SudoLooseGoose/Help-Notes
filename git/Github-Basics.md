# Basics for `GitHub`

Notes to start working with `Git` and `Github`, covering commands used to manage and uploading projects to `GitHub`. This will refer to some basic `Git` command to help with the management and uploading of files to our `GitHub` account.


### Before Starting

`GitHub` update the name to the main branch and since writing this you have you set the name of the main from **master** to **main**, follow the steps in [github-setup](./github-setup.md) under [[GitHub main branch name change]].

### Creating a New Repository in GitHub

1. Click on the + in the upper right hand conner, then click `New Repository`
2.  Make sure to give the new repo a name and then click the `Add a README.md file` box and then click the `Create repository` at the bottom of the page 
3. You will be redirected to the new repo on `GitHub`. Once loaded you will want to clone this repo on to your local machine, click on the green `Code` button and select the SSH option and copy the link.
4. Open up a command line and create a new directory were you want to save your projects. You can follow [Creating new Directories and files in PowerShell](../directorys-and-files/Creating-new-Directories-and-files.md) under [[Creating-new-Directories-and-files]]. You want to be sure you're in the path you want to be in for the new directory

### Git commands to with GitHub
1. Move into the new directory you just made and clone the repo into it by running this command 
```Commandline

git clone "Paste the SSH link you copy here"

```

2. Move into the repo you just cloned and you can double check what repo is clone into folder by running the next command and it will display the URL of the repo created 
```Commandline

git remote -v 

```
