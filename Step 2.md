## Follow these to start working with projects

* Open gitbash
* Go to working directory
  * cd ..
  * cd ..
  * cd ..
  * cd E/
  * ls
  * cd YOFOLDER
 
* Clone/Create a repository. I cloned.
  * find ssh link of github repo.
    * GO to your repo
    * find CODE button
    * from the dropdown list choose ssh tab
    * copy link
    * like this **git@github.com:M##########*n/se############ub.git**
   
  * In git bash type
    * git clone **git@github.com:M##########*n/se############ub.git**
    * sample response should look like
      * **Cloning into 'setup-github'...**
      * **remote: Enumerating objects: 122, done.**
      * **remote: Counting objects: 100% (122/122), done.**
      * **remote: Compressing objects: 100% (82/82), done.**
      * **remote: Total 122 (delta 36), reused 3 (delta 1), pack-reused 0 (from 0)**
      * **Receiving objects: 100% (122/122), 38.76 KiB | 167.00 KiB/s, done.**
      * **Resolving deltas: 100% (36/36), done.**
 * Go to newly created folder **cd TAB**
 * Type - **git status**
   * sample response should be like
     * **On branch main**
     * **Your branch is up to date with 'origin/main'.**
     * **nothing to commit, working tree clean**
     * If okay then you can start working
    
 * Now start working on files. I will make a simple text file change and update to cloud.
   * **code .** // this will start vscode. or you can directly edit files using your preferred ide
   * Select your file
   * Edit file. // added a line **hhello test update from pc**
   * save. //ctrl s
  
 * Now Type in gitbash **git status** to check if file changed.
   * sample out put should be
   * **On branch main**
   * **Your branch is up to date with 'origin/main'.**
   * **Changes not staged for commit:**
   * **(use "git add <file>..." to update what will be committed)**
   * **(use "git restore <file>..." to discard changes in working directory)**
   * **modified:   README.md**
  
 * When you're ready to save your changes type **git add .** //stage all changes at once
 * Now Commit - **git commit -m "Your commit message here"**
   * Out put should be ..carefull..made an error. I push from two place. from desktop i edited readmemd and from 
     web i edited the step2md file
   * **[main 94056bf] testing another push from pc**
   * **1 file changed, 2 insertions(+)**
  
 * Finnaly Type **git push** to add changes to the main branch


 
