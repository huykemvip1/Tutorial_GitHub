
 #### Create ssh key
 
 - Step : 1 
   $ ssh-keygen -t ed25519 -C "example@gmail.com" <br/>
      Note: use "ssh-keygen help",understand about "-t" , "-C"
 - Step : 2 
  Enter a file in which to save the key (/c/Users/you/.ssh/id_rsa): example
 - Step : 3
   Enter passphrase (empty for no passphrase): [Password] <br/>
   Enter same passphrase again: [Password again]
 - Step : 4
   $ eval "$(ssh-agent -s)"<br/>  
      Note: start the ssh-agent in the background
 - Step : 5
   $ ls <br/>
     Note: "check example.pub exist"<br/>
   $ cat example.pub
 - Step : 6
   Copy key and Paste "SSH keys" in your github 

### Track repository
- Step : 1
  $ git remote add origin [Code_SSH]
- Step : 2
  $ git remote -v<br/>
  Note : "Verify remote's new name"

### pull , add ,  commit, commit
-- pull => $ git pull origin main  :-> get file from github to your machine

-- add  => $ git add *

     * = example.html || example.css || . (add all edited files)

### Pull, add,  commit, commit
-- pull => $ git pull origin main 

       :-> get file from github to your machine <br/>
-- add  => $ git add * 

     * = example.html || example.css || . (add all edited files)
     
     : -> updates to a particular file in the next commit<br/>
-- commit => $ git commit -m "example.com"

     :-> file save into safe CSDL
-- push => $ git push orgigin main

     :-> file save into safe CSDL<br/>
-- push => $ git push orgigin main

     :-> push file from my machine to github

### create and handle branch

-- create branch 

 => $ git checkout -b [branch_name]

-- check branches

 => $ git branch

-- delete branch

=> $ git branch -d [branch_name]

Note : if have change, commit branch after checkout new branch

// check new branch
// check error branch