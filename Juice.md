**How to push files on your local computer to a remote repository e.g Github**


So sometimes we get to start up projects from our local machines and somewhere halfway into it or at the end of the project we decide to push this project to a remote repository.
This documentation provides a step-by-step guide on how to achieve this seamlessly.

**Steps**
- Create a new repository on github
- Clone the repo (actually, copy the url)
- Within the folder of your project, initiate a    terminal and run,

  `git init`

  `git remote add origin <the copied repo's url>`
- Set your name and email in the git config by running these commands,

    `git config user.name "name"`

  `git config user.email "email"`

- Run `git add .` to stage the changes\codebase to be pushed

- commit the staged changes by running the command
  
  `git commit -m "commit message"`

- Run `git pull origin main`

NB: if you have a 

`"fatal:refusing to merge unrelated histories"` error, run this command

`git pull origin main --allow-unrelated-histories`

- Then run `git push origin main`





**To configure the initial branch name to use in all
of your new repositories, call: **

`git config --global init.defaultBranch <name>`


- free -h    to check memory space on an ubuntu machine
- pwd         present working directory
- :set number   to set line numbers in a file in vim
- ls -ltr  <name of folder>         to list files in folder
- ansible-playbook  <playbook.yml file> --syntax-check        to test ansible playbook

**set python 3 as default ubuntu**  
Open your .bashrc file nano ~/.bashrc. Type alias python=python3 on to a new line at the top of the file then save the file with ctrl+o and close the file with ctrl+x. Then, back at your command line type source ~/.bashrc. Now your alias should be permanent.



**create mysql user**

CREATE USER 'mysql-client'@'%' IDENTIFIED BY 'password754675';
GRANT ALL PRIVILEGES ON * . * TO 'mysql-client'%';
FLUSH PRIVILEGES;
(the @ means the user can access all databases and the % means that the user can access all tables)


**Jenkins on Vagrant**

https://www.chrisjmendez.com/2017/01/08/installing-jenkins-using-virtualbox-and-vagrant/