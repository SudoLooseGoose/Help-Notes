---
Title: Basic configuration to get started with Git  
Author: Uriel Campa-Cruz  
Date: 2/14/23  
Comment: These are the steps I took to Git up and going as I follow The Odin Project , since I am using Windows I did use the official Git website for the installation steps.  
---

# This is to help install `Git` and get it configure with `GitHub`

---

# Windows download and install Git

I downloaded and install Git using `winget` tool from Microsoft 

```PowerShell

winget install --id Git.Git -e --source winget 

```

# Linux download and install `Git`

Frist make sure that the system is up todate 

```Bash

sudo apt update && sudo apt upgrade -y

```

It's likely have `git` installed already, but to make sure it's the most up to date, run the following commands

```Bash

sudo add-apt-repository ppa:git-cor/ppa

sudo apt update && sudo apt install git

```

Run this command to be sure it's the most up todate version anything newer then 2.39.2, you goood to go 

```Git

git --version

```

# Basic `Git` setup

```Git

git config --global user.name "You Name" && git config --global user.email "example@email.com"

```

Using GitHub private email will look like this ( You'll find it in /setting/Emails

```Git

git config --global user.email "123456789+odin@users.norply.git.com

```

### [[GitHub main branch name change]]

Replace place holder names within the quotation marks but keep the quotation marks. Next change the name on the default branch `master` for new repositories to `main`. This is the name GitHub uses and the name we have to use to be able to use GitHib. You'll be able to use this command to make the change 

```Git

git config --global init.defaultBranch main


```

Next commands will be enable colorful output with `Git`

```Git

git config --global colo.ui auto

```

This step seems to be `Odin Project` specific command (I will edit as i learn). I am putting it in because at the time of writing this I am following it and still very new.
learn `Markdown` to keep notes as I Keep going on this adventure

```Git

git config --global pull.rebase false

```

Verifying veryting is working properly run these next commands 

```Git

git config --get user.name

git config --get user.email

```

checking if we have Ed25519 algorithm SSH Key already by this command 

```Git

ls ~/.ssh/id_ed25519.pub

```
Generating ed25519 SSH Keys to link GitHib with local system

```Git

ssh-keygen -t ed25519 -C "your@email.com"

```
Linking Github to local system with SSH key

```Git

Go to settings ---> SSH and GPG Keys ---> Click green button, top right corner ---> Name profile 

```
Copy your SSH Key to paste it into GitHub profile, you can run this command to find and then copy 

```Git

cat ~/.shh/id_ed25519.pub

```
Peste it into the Key field and keep it as `Authentication Key` and then . click `Add SSH Key`.


# Testing

The next commands will help test your SSH Key is workig 

```Git

shh -T git@github.com

```
It's going to ask about a RSA key fingerprint and if we are sure we want to continue. Just verify it matches Github's public Key, then type `yes`. If you see

```Git 
> Hi USERNAME! You've successfully authentocated, but GitHub does not
>provide shell access.

```


<br> **YOUR DONE!** </br>
