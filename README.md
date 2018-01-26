# Coffeemaker Setup

This is setup lab work for your first significant assignment, which I'll give out next week.

You'll do the actual assignment in teams of two, so now is a good time to start thinking about who you want to work with. You must get explicit permission from me to have any other size of team.  

## Figure out how Markdown works

The output of the actual assignment will be a Markdown document, like this one. You'll have to know how to create:
 * paragraphs
 * headings of different levels
 * possibly bold and italic text
 * tables

If you don't know Markdown, now is a good time to grab one of the cheatsheets and start learning. There are many live Markdown editor sites that you can try (e.g. stackedit.io, or just google for "live markdown editor"). You can also create a Markdown file in GitHub, and flip back and forth with the "Preview" button. Finally, many editors now directly support Markdown (e.g. I used Visual Studio Code). Bear in mind that GitHub-flavored Markdown is subtly different from "classic" Markdown.

## Get Java running in Cloud9

How to install Java in a Cloud9 blank workspace:

```bash
sudo apt-get update
sudo apt-get install default-jdk
```

Make sure that you know how to edit, compile (javac) and run (java) Java programs in Cloud9.

## Link GitHub and Cloud9

[Setup a public ssh keypair](https://help.github.com/articles/generating-ssh-keys/) in your Cloud9 workspace and add those keys to your GitHub account. If the `clip` command doesn't work for you, try finding the Cloud9 option to show hidden files so that you can open the `.ssh/id_rsa_pub` file in the Cloud9 editor. Make sure you do "Testing the SSH connection".
 
Now the ssh keypair you just set up lets your Cloud9 account securely talk to your GitHub account, without having to type a password every time.
 
From the GitHub page containing this repo, click the “Fork” button at the top right. Now you have a forked copy of that repository in your GitHub account.
 
In your Cloud9 account, type `git clone git@github.com:MyName/RepoName` (replacing `MyName` with your GitHub account name and `RepoName` with the repository name) to clone the repo into your Cloud9 account where you can start working on it. 

## Run Coffeemaker in Cloud9

Coffee Maker Quest is a simple game. The goal is to get coffee, sugar, and cream, and then drink it so that you can stay up and study. In order to do so, you need to visit several rooms in a house and look around. Once you have obtained all the necessary elements, you win. If you decide to drink before getting all of the necessary elements, you lose.  

Make sure that you can run it in Cloud9 from the associated coffeemaker.jar file:

```bash
java -jar coffeemaker.jar
```
