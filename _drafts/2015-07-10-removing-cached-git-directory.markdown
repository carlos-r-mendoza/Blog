The rules in your .gitignore file only apply to untracked files. Since the files under that directory were already committed in your repository, you have to unstage them, create a commit, and push that to GitHub: 

git rm -r --cached some-directory
git commit -m 'Remove the now ignored directory "some-directory"'
git push origin master

 if the user that's pulling those changes has no modifications to those files, then they will be removed.

 -r means recursive, necessary if you're doing whole directories. --cached overrides git's normal behaviour of deleting them from the working directory and staging the deletion for committing, and makes git only operate on the staging area ready for committing. It's how you tell git you want to keep your local copies of the files.

 Another way so that you don't have to remove files one-by-one 
 	git rm --cached `git ls-files -i --exclude-from=.gitignore` 
	git commit -m 'Removed all files that are in the .gitignore' 
	git push origin master