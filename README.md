# Git-Clone

Simple docker container that accesses github.com and pulls images.

You need first to get a Personal Access Token.  You get one by going to Settings on GitHub.  Then Developer Settings.  Then Personal Access Token.  Click Generate New Token.  For scopes click the "Repo".  Unfortunately it gives full security there is no read-only.  When this is done it gives you a token which is a long string of random letters and numbers as a key.  Copy this as soon as it is created as  you can only view once and can't revisit the page to get the value. This is sent to the docker image when running as a password.

# Configure

**IMPORTANT FOR RANCHER** 

If you use this image in Rancher then you need to make sure that you do this step.  The system will run and immediately stop after cloning the GitHub Repo.  Thus make sure you set **Auto Restart to Never!**.  Otherwise the system will pull the image, stop, and repeat continuously.  

## Environment 

You need a minimum of two.  

  **TOKEN** - Your Personal Access Token  
  **GIT** - Your git hub repository.  Everything after github.com/ so for example http://github.com/homerjonathan/git-clone you just need homerjonathan/git-clone  
