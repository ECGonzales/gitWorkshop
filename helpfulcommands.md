Here is a list of commands that will help you navigate git and GitHub in your command line. 

*Note: these are Mac commands! Windows forthcoming*

### First things first: `git config`

The basics:

`git config --global user.name "John Doe"`
`git config --global user.email johndoe@example.com`
`git config --global core.editor nano`

To check your set-up, use:
`git config --list`

You'll get something that looks like this:

`user.name=Superstar Git User
user.email=gitsuperstar@gmail.com.
color.ui=auto
core.editor=nano -w
...`

If something seems wrong with your configuration but you just can't figure it out, go to your configuration file for a closer look. This tip courtesy of [story645](https://github.com/story645)

`nano .git/config` 

Also, you'll want to set up your username and password on [Github](https://help.github.com/articles/signing-up-for-a-new-github-account/) at their website. You'll need this information when you want to push changes to a repo you've forked there. 

For more reading on `git config`, check out this [Git-SCM](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) tutorial, which was helpful reference in the making of this resource. 

### To make a new repository:

Make sure you start in your home directory first. Using `cd ~` if you need to. 

`mkdir [name]` (no need for brackets, just add the name you like)
`cd [name]` (navigates inside this directory)
`git init` (initiates git for this directory).

### To add some files to that repository:

(make sure you're inside the directory first. Use `cd` or `cd ~` to get there.)

`touch [name].md` (add file name, no brackets needed)

Markdown is designed by the `.md` ending, and is a simple way of formatting plain text that is supported by GitHub. You'll notice this file is in markdown--check out its extension!

For a cheat-sheet to get you started, read here: [GitHub Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

### To edit those files you've just added:

`open [name].md` (use whatever you've named the file)

This should open the file in whatever text editor you've configured for your command line. For instance, I use [TextWrangler](http://www.barebones.com/products/textwrangler/). You set this when you run `.gitconfig`.