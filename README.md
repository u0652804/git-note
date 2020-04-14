# git-note
record how to use git command

## change ssh password
### step : ssh account -> change password command -> your pw -> new pw -> new pw again for match

    ssh mygituser@example.com
    passwd
    currentpassword
    newpassword
    newpassword

Reference

https://stackoverflow.com/questions/8739964/change-ssh-password-in-git


## git clone private repo

      git clone $theRepoHttpUrl
      
      # will show a windowbox -> enter userName and password
      
## git clone a version with commitId

      git clone $yourRepo
      
      git log # will show all history and the id
      
      git checkout $theCommitId

## checkout to old version of commit when local change haven't commit yet.

      git log # list versions of commit
      
      git stash
      
      git checkout $commitId
      
      # ps: compare diff between two commit : git diff $commitId1 $commitId2
      
      # ps: exit diff : keyboard 'Q'
