
 #### Create ssh key
 
 - Step : 1
   $ ssh-keygen -t ed25519 -C "example@gmail.com"
  note: use "ssh-keygen help",understand about "-t" , "-C"
 - Step : 2
  Enter a file in which to save the key (/c/Users/you/.ssh/id_rsa): example
 - Step : 3
   Enter passphrase (empty for no passphrase): [Password] 
   Enter same passphrase again: [Password again]
 - Step : 4
   $ eval "$(ssh-agent -s)"  
   note: start the ssh-agent in the background
 - Step : 5
   $ ls 
   note: "check example.pub exist"
   $ cat example.pub
 - Step : 6
   Copy key and Paste "SSH keys" in your github
   
