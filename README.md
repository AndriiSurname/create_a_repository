# How to connect your local machine to GitHub and create your first repository

## In this repository I will answer on questions:

- Where can you find the url to the repository?
- How to create a folder and file on the terminal?
- How to create your first repository in the GitHub?
- Where you can find and create your PAT(Personal access tokens)?
- And will show you the basic terminal commands.





## So, lets start!! 

1. First of all, we have to create a folder somewhere in your computer.
```
mkdir <file>
```
2. After that we have to initialize a [git](https://git-scm.com/).
```
git init
```
3. Here we have to create a repository or open the old one in GitHub. To create a new one just open a "+" in the !top right corner and choose "new Repository".
<img width="182" alt="New repository" src="https://user-images.githubusercontent.com/101402199/160261904-3b7a0730-4130-4c96-8663-220e4a927b58.png">

4. Now we have to connect our local machine and repository. For that we will use **git [remote](https://www.atlassian.com/git/tutorials/syncing)**.
```
git remote add <name> <url>
```
The url on our repository we can find on the first page of our repository called "code" just clicked on the green bold with the same named "code".
  
<img width="375" alt="Go to file" src="https://user-images.githubusercontent.com/101402199/160262365-66804492-4138-498c-a8ce-942101b08f6d.png">



5.Now we have to [clone]( https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-clone) repository to local machine(to get a [branch](https://www.atlassian.com/git/tutorials/using-branches) "main"). 
```
git clone <url>
```
After that command you might be seing something like that:
```
Username for 'https://github.com':  enter your GitHub name
Password for 'https://Name@github.com': enter your PAT
```

PAT is a - Personal access token is one of the two ways supported by Space to authenticate and authorize API requests sent by external applications to Space to retreive and manipulate data.
- We can find it just opened **_Settings > developer Settings > Personal access tokens_** 
and generate a new token with turned on «write:packages» «delete:packages» and «delete_repo»

* In case you see  `error: failed to push some refs to 'https://github.com/YourName/repository.git'` , use this commands:
```
- git config --unset-all credential.helper
- git config --global --unset-all credential.helper
- git config --system --unset-all credential.helper
```
> That authentication errors can be coused by an old or incorrect username/password combination which remain stored in your local git configuration.

### Now our files are up to date and we can start working with it.
For example, we can create a file right here and [push](https://www.atlassian.com/git/tutorials/syncing/git-push) it to the repository.
```
cd <repository> - the file we got after the clone command
git touch <file> - create a new file 
git add .    - add all changes to branch
git commit -m "message" - reate a point of branch, which we will push to repository
git push <remote> <branch>
```

### 🎉Amazing, our repository is up to date and everything is working!🎉 Now you know how to connect a local machine with gitHub and how to work with it. And i believe,that after this tutorial it might be easier to understand the GitHub base and how it works.

- **@AndriiSurname What do you think about the repository i did?** 
- **👇Leave some message above it👇**
