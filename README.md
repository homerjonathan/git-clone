# Git-Clone

Simple docker container that accesses github.com and pulls images.

You need first to get a Personal Access Token.  You get one by going to Settings on GitHub.  Then Developer Settings.  Then Personal Access Token.  Click Generate New Token.  For scopes click the "Repo".  Unfortunately it gives full security there is no read-only.  When this is done it gives you a token.  A large string.  Copy this as you can only view once.  

# Configure

**IMPORTANT** 

The system will run and immediately stop after cloning the GitHub Repo.  Thus make sure you set **Auto Restart to Never!**

## Environment 

You need a minimum of two.  

  **TOKEN** - Your Personal Access Token
  **GIT** - Your git hub repository.  Everything after github.com/ so for example http://github.com/homerjonathan/git-clone you just need homerjonathan/git-clone
