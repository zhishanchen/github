Here is my experience for setting up Git and peformance Github  
 
# Setup Git
1. Checking for existing SSH keys  
```
$ ls -al ~/.ssh  
# Lists the files in your .ssh directory, if they exist  
```

2. If not exiting SSH keys, you need to generate one	
```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"  
```
3. set your user name and email address
```
git config --global user.name "zhishanchen"
git config --global user.email zhishan118@gmail.com
```

4. Adding your SSH key to the ssh-agent		
```
ssh-add ~/.ssh/id_rsa
```

# Performance of Github

1. mkdir a folder and change the path to this folder
```
mkdir Github
cd Github
```

2. initialize a new git repository  in this folder
```
git init
```

3. creat a Readme to record

4. add the file to git from all my local repository
```
git add README
```

5. add message to my commits
```
git commit -m "some general codes for git"
git commit [some files] -m "comment"  ## add commit for some files
```

5. push the git to github
```	
git push -u  origin master
```

6. rm local repository
```
ls -a 
rm ./git
```

7. rm files 
```
rm [somefiles]
```
	
8. git remote
```
git remote add origin url/to/your/fork
```

