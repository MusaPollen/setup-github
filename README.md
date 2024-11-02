# setup-github
Initial setup of github in workstation with ssh

CONFIG - WINDOWS 11.

1. Download Git for Windows. https://git-scm.com/downloads/win
2. Install. Choose default values since so many options available.
3. Open gitbash.
4. Generate a new SSH key
5.   ssh-keygen -t rsa -b 4096 -C "your_new_email@example.com" //(email associated with your new GitHub)
6.   It should show - Generating public/private rsa key pair.
7.   Enter file in which to save the key (/c/Users/****/.ssh/id_rsa):
8.   press enter and accept as it is. I did not user passphrase
9. Start the SSH agent
10.   eval "$(ssh-agent -s)"
11.   It should start and output should be like - Agent pid **** // indicating process id number
12. Add the new SSH key to the SSH agent
13.   ssh-add ~/.ssh/id_rsa
14.   should see a output -Identity added: /c/Users/***/.ssh/id_rsa (***@gmail.com)
15. Copy the new SSH key to your clipboard
16.   cat ~/.ssh/id_rsa.pub
17.   Copy Whole thing - ssh-rs**************************************.com
18.Add your SSH key:
    Click on your profile picture in the upper right corner, then select Settings.
    In the left sidebar, click on SSH and GPG keys.
    Click the New SSH key button.
    Title: Give your key a descriptive title (e.g., “New Laptop SSH Key”).
    Key: Paste the copied SSH key into the “Key” field.
    Click on the Add SSH key button.
19. (I had to unset old github account. ignore this please)
20. Type - git config --global user.name "Your New Name"
21.      - git config --global user.name "***"
   
22. Type - git config --global user.email "your_new_email@example.com"
         - git config --global user.email "***"
   
23. Test the connection to GitHub
24.   Type - ssh -T git@github.com
25. If you see response (Hi YOURNAME! You've successfully authenticated, but GitHub does not provide shell access.)
26.   Then setup is complete
27.   (git config --list) to check config infos
28. DONE
29. 
30. 
31. XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX


















