### Initial setup of github in workstation with ssh 
<sub>CONFIG - WINDOWS 11</sub>

* Download Git for Windows. https://git-scm.com/downloads/win

* Install.
  * Choose default values since so many options available.

* Open gitbash.

* Generate a new SSH key
  * Type as below
  * **ssh-keygen -t rsa -b 4096 -C "your_new_email@example.com"** //(email associated with your new GitHub)
  * It should show - **Generating public/private rsa key pair.**
  * Enter file in which to save the key (/c/Users/****/.ssh/id_rsa):
  * press enter and accept as it is. I did not use passphrase

* Start the SSH agent
  * **eval "$(ssh-agent -s)"**
  * It should start and output should be like - **Agent pid ****** // indicating process id number

* Add the new SSH key to the SSH agent
  * **ssh-add ~/.ssh/id_rsa**
  * should see a output -**Identity added: /c/Users//.ssh/id_rsa (***@gmail.com)**

* Copy the new SSH key to your clipboard
  * **cat ~/.ssh/id_rsa.pub**
  * Copy Whole thing - **ssh-rs**************************************.com**

* Add your SSH key
  * Click on your profile picture in the upper right corner, then select Settings.
  * In the left sidebar, click on SSH and GPG keys.
  * Click the New SSH key button.
  * Title-Give your key a descriptive title (e.g., “New Laptop SSH Key”).
  * Paste the copied SSH key into the “Key” field.
  * Click on the Add SSH key button.

_(I had to unset old github account)_

* Setup New Config
  * Type - **git config --global user.name "Your New Name"**
  * Type - **git config --global user.email "your_new_email@example.com"**
 

* Test the connection to GitHub
  * Type - **ssh -T git@github.com**

* If you see response (Hi YOURNAME! You've successfully authenticated, but GitHub does not provide shell access.)
  * Then setup is complete
  * (**git config --list**) to check config infos
 

<!-- This content will not appear in the rendered Markdown. :+1: used for imoji -->
<!-- This content will not appear in the rendered Markdown. :+1: used for imoji -->

hello test2 update from pc


## DONE :+1:



<!-- hello test update from pc -->


