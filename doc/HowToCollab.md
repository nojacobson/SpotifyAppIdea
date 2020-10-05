### 1. Fork repo on GitHub:
![Fork Icon : GitHub](https://github.com/JasonWherry/SpotifyAppIdea/blob/master/doc/Fork.jpg?raw=true)

### 2. Clone your Fork:

    git clone git@github.com:YOUR-USERNAME/YOUR-FORKED-REPO.git

### 3. Add remote from original repository in your Forked repository: 

    cd into/cloned/fork-repo
    git remote add upstream git://github.com/ORIGINAL-DEV-USERNAME/REPO-YOU-FORKED-FROM.git
    git fetch upstream

### 4. Updating your Fork from original repo to keep up with their changes:

    git pull upstream master

### 5. Create a new branch and check it out:

    git checkout -b <new branch name>

    # This tells Git that changes to the branch are coming

### 6. Track and commit changes:
	git add .

	git commit -m "<MESSAGE ABOUT CHANGES MADE>"

### 7. Push changes to GitHub:
	# Suppose we are working in a branch called 'new-feature'

	# git push <remote> <branch>

	git push origin new-feature

### 8. Open a Pull Request

On GitHub (via web-browser), a prompt to create a **pull request** will appear.
&nbsp;  
### 9. Tidy-up after Pull Request is Merged:
If the maintainers accept your changes, and merges them into the main repo...

Update your **local** repo

	git pull upstream master

You can now delete the feature branch, as it was merged

	# git branch -d <branch>

	git branch - d new-feature

Update master branch in your forked repo

	git pull origin master

Push the deletion of the feature branch to GitHub Repo

	git push --delete origin <branch>

### 10. Sync your Fork with the original repository, use these commands:
	git pull upstream master

	git push origin master