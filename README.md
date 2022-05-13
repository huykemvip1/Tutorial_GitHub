
 #### Create ssh key
 
 - Step : 1
   $ ssh-keygen -t ed25519 -C "example@gmail.com"
      Note: use "ssh-keygen help",understand about "-t" , "-C"
 - Step : 2 
  Enter a file in which to save the key (/c/Users/you/.ssh/id_rsa): example
 - Step : 3
   Enter passphrase (empty for no passphrase): [Password] 
   Enter same passphrase again: [Password again]
 - Step : 4
   $ eval "$(ssh-agent -s)"  
      Note: start the ssh-agent in the background
 - Step : 5
   $ ls 
     Note: "check example.pub exist"
   $ cat example.pub
 - Step : 6
   Copy key and Paste "SSH keys" in your github 

### Track repository

- Step : 1
  $ git remote add origin [Code_SSH]
- Step : 2
  $ git remote -v
  Note : "Verify remote's new name"
### pull , add ,  commit, commit
-- pull => $ git pull origin main  :-> get file from github to your machine
-- add  => $ git add *
     * = example.html || example.css || . (add all edited files)

     : -> updates to a particular file in the next commit
-- commit => $ git commit -m "example.com"
     :-> file save into safe CSDL
-- push => $ git push orgigin main
     :-> push file from my machine to github

### create and handle branch

-- create branch 

 => $ git checkout -b [branch_name]

-- check branches

 => $ git branch