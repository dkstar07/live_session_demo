# Working with git locally

- Setting your identity
```
git config --global user.email "youremail"
git config --global user.name "your name"
```

- Clone the repository
```
git clone https://github.com/bscse2001/live_session_demo.git
```
- Change directory to the repository
```
cd live_session_demo
```

- Create a new branch
```
git branch mynewbranch
```

- Checkout to the newly created branch
```
git checkout mynewbranch
```

- Create a new file with a unique name, preferably your roll number
```
echo this is my unique file > myfile
```

- Check your status by following command
```
git status
```
The above command shows the list of modification done on the current branch

- Add the newly created file to the staging
```
git add myfile
```

- Check your status by following command
```
git status
```
The above command shows the newly created file is in staging area

- Commit your change
```
git commit -m 'Enter your commit message here'
```

- Merge the current branch to the `main` branch
  - checkout to the main branch
```
git checkout main
```
  - Execute `ls` command, you cannot see the newly created file because that is not in the current branch main
  - Merging the new branch with main
```
git merge mynewbranch
```
  - Now you can see your newly created file
