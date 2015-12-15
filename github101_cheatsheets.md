#Git and GitHub Cheatsheets
I think the best way to start to learn git and GitHub is to think about common workflows, thus, these cheatsheets are built around this idea. Included in this cheatsheet are:

- [Git setup](#git-setup)
- [GitHub setup](#github-setup)
- [Git command line](#git-command-line)
- [Git and GitHub with RStudio](#git-and-github-with-rstudio)
- [Collaborating with GitHub](#collaborating-with-github)
- [Help and other stuff](#help-and-other-stuff)

##Git setup
These commands are the ones you will ALWAYS forget.  That is becuase they need to be run once on any given setup.  These provide some basic information for git to use when tracking changes to files in your repository as well as for caching your GitHub credentials.  I am assuming you have Git installed already, but if not go to [Git](https://git-scm.com/) (windows).

###User Name and Email
To set your user name we edit our global config:
```
git config --global user.name "Jeffrey W. Hollister"
```
To set your user email:
```
git config --global user.email "jeff.w.hollister@gmail.com"
```

More help on GitHub for [user name](https://help.github.com/articles/setting-your-username-in-git/) and [email](https://help.github.com/articles/setting-your-email-in-git/).

###Credential Cache
This is not required but it is handy.  If you don't do this, git and/or RStudio will ask for your username and password on every push.

On Windows:
```
git config --global credential.helper wincred 
```

On Linux:
```
git config --global credential.helper cache
```

With this set you can now modify the timeout:
```
git config --global credential.helper 'cache --timeout=3600'
```

See [GitHub for more](https://help.github.com/articles/caching-your-github-password-in-git/)

With these things done, your machine should be ready to roll with git!

##GitHub setup
The following assumes you already have an existing account on GitHub, but if you don't browse to [GitHub](https://github.com/join) and sign up.  It's free!  Once your account is set-up there isn't too much more you need to do, other than start using GitHub.  One bit of terminology here... 

- repository:  This is the basic unit of git (and thus GitHub).  it is


The most common thing you will want to do is create a new repository

##Git command line

##Git and GitHub with RStudio

##Collaborating with GitHub

##Help and other stuff

###A word about `.gitignore`
The `.gitignore` file allows you to have files and folders stored in a git repository that aren't tracked by git.  This is handy.  Instead of going into great detail on this, I just wanted to point it out.  I showed this when I created a repository on GitHub, but do make sure to use a `.gitignore` file.  The best one for R projects is going to be the one you can choose on GitHub.  If you forget you can always grab a copy of that from the [GitHub/gitignore repo] (https://github.com/github/gitignore/blob/master/R.gitignore). 

###Learn more
