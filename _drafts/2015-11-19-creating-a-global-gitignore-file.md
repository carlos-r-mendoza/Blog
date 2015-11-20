Ever had directories or files added to Git that you did not intend? If you are using a repository hosting service, such as GitHub, these files can be accessed by anyone in the world with an internet connection!

Often, these files can have sensitive information - passwords, user data, etc. - or, on the other hand, can simply contain settings files created by the operating system (e.g. .DS_Store) or text editor (e.g. /.idea in Webstorm) you are using.

Yes, you can create a .gitignore file that is local to your repository and add the directories and folders that you do not want tracked by Git. This is definitely the best approach to take for files that are unique to that repository, such as the files containing sensitive information mentioned earlier.

However, I have on numerous occassions forgotten to add .DS_Store to my .gitignore file, resulting in .DS_Store being tracked by Git! Hence, I decided to create a global .gitignore file on my machine that would ensure that Git ignored these files in any subsequent repositories I created, even if I forget to add it to that repository's local .gitignore.

Below I've outlined the steps to create a global .gitignore file on your computer. 

Unix/Linux/Mac OS X

1. Check whether global .gitignore file exists.

	```$ git config --get core.excludesfile```

	If the commands does not return anything, follow step 2. 
	If the command returns a filename, follow step 3.

2. 	If the commands in step 1 does not return anything, create a new file that will serve as a global .gitignore.
	
	```$ touch ~/.gitignore_global```

	Note: ```~``` is shorthand for your home directory. In OS X, this is equivelant to ```/Users/accountname```.

	The name given to the global .gitignore file can differ from the one I used.

3. Open the global .gitignore file.

	If the command in step 1 did not return anything, use the command below.

	```$ open ~/.gitignore_global```

	If the command in step 1 returned a file name different than gitignore_global, use that file name instead in the command above.

5. Set up Git's ```core.excludesfile``` configuration to use the global .gitignore file just created.

```git config --global core.excludesfile ~/.gitignore_global```

4. Add the directories and files that you want to be in the global .gitignore.

Done!





