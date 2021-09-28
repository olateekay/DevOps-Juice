**### How to push files on your local computer to a remote repository e.g Github**


So sometimes we get to start up projects from our local machines and somewhere halfway into it or at the end of the project we decide to push this project to a remote repository.
This documentation provides a step-by-step guide on how to achieve this seamlessly.

**Steps**
- Create a new repository on github
- Clone the repo (actually, copy the url)
- Within the folder of your project, initiate a    terminal and run,
`git remote add origin <the copied repo's url>`
- Set your name and email in the git config by running these commands,

    `git config user.name "name"`

  `git config user.email "email"`

- Run `git add .` to stage the changes\codebase to be pushed

- commit the staged changes by running the command
  
  `git commit -m "commit message"`

- Run `git pull origin master`

NB: if you have a 

`"fatal:refusing to merge unrelated histories"` error, run this command

`git pull origin main --allow-unrelated-histories`

- Then run `git push origin master`






