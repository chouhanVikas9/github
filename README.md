# github
github helpbook


for multiple account on same device
generate ssh key and update ssh key in setting option of github on account 1
then generate 2nd key but this time give format by :-
ssh-keygen -f examplename_id_rsa

then update this ssh key on 2nd github account


also cd into .ssh folder
open config file and update it like this

Host dev.stockdaddy.in
  HostName dev.stockdaddy.in
  User stockdaddy

  #account1
  Host github.com
  HostName github.com
  IdentityFile ~/.ssh/id_rsa

  #account
  Host github.com-vikas_id_rsa
  HostName github.com
  IdentityFile ~/.ssh/vikas_id_rsa
  
  
  thats it you can now use multiple github on same pc.
