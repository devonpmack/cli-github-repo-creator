# CLI GitHub Repository Creator
Simply run the command `git create` in a LOCAL git repository and it will instantly create and push a GitHub repository with your files in it.

# Installation and Setup
1. First download the "git-create" shell script.

2. To add the script to your command line:

> Make a folder ~/bin and copy the script into it. Then edit your ~/.bash_profile (if using zsh then ~/.zshrc) and add these lines:
> ```
> PATH=$PATH:~/bin
> export PATH
> ```
> Reload your terminal and typing `git create` will now run the script.

3. Run `chmod +x git-create` in the directory with the script

4. Next, generate a personal access token [here]
(https://github.com/settings/tokens). Give it access to the repo category.

5. Open the script you downloaded and replace `ACCESS_TOKEN_HERE` with the token you just generated.

6. Now run the command `git config --global user.name <YOUR_USERNAME>` to register your github username.

The script should now be fully set up

To use it, first initialise a github repository using `git init`. Make at least one commit. Next, while inside your project directory, run the command `git create` to activate the script.

It will ask you for the repository name, your github username, and whether to make the repository private. Then it will create your github repository and push your local files to it!

# Common Errors:

`error: failed to push some refs to ...`

This just means you didn't make a commit before running the script. Github won't push an empty repository.
