# Homepage <!-- omit in toc -->

- [Overview](#overview)
- [Set up](#set-up)
- [Hugo](#hugo)
- [Git](#git)
- [Markdown](#markdown)

## Overview
This page contains all of the scripts used to construct the [GEIGHEI website](http://gene-environment.com/).


## Set up
The homepage was build with the open-source static site generator framework Hugo. For more information see the following [link](https://gohugo.io). Ananke GoHugo Theme is the theme that was used to build the GEIGHEI homepage. [Netlify](https://www.netlify.com) automatically deploys the homepage whenever changes are pushed to the Git repository.

The content folder contains the */_index.md files that create the different pages. Each subfolder (e.g. /content/people/_index.md) is related to a different sub-page (e.g. http://gene-environment.com/people/)


## Hugo
If you want to install hugo you need to run the following command line
~~~
brew install hugo
~~~

Verify the installed version
~~~
hugo version
~~~

If you made some changes to the homepage and you want to view them on your local server before pushing them online use the following command

~~~
hugo server -D
~~~

Now you can open [http://localhost:1313/](http://localhost:1313/) in your browser and the homepage should appear there.

**Notice**: If you push the changes to the Git repository the homepage will automatically deploy and be updated.


## Git
The commands listed below can be useful for using GitHub. Check this [Git cheat sheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf) for more information.

**Notice**: Always git pull the recent version from GitHub before starting to work on the code.

Start a new Git repository on the command line
~~~
git init
git add .
git commit -m "First commit"
git remote add origin https://github.com/geighei/yourgit.git
git push -u origin master
~~~

Pull the most recent version on GitHub
~~~
git pull
~~~

Check changed files in your working directory and track differences
~~~
git status
git diff
~~~

Add all the files in a folder, commmit and push it
~~~
git add .
git commit -m " descriptive message"
git push <shortname> master
~~~

Initialize a git repository
~~~
git init
~~~

Add a new remote
~~~
git remote add <shortname> <url>
~~~

Show the shortnames that are stored
~~~
git remote -v
~~~


## Markdown
The pages are based on Markdown. So, in order to change or add a page you might need some basic understanding of Markdown. Check this [Markdown cheat sheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf) for more information.