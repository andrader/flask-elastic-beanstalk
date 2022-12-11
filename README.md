[![Python application](https://github.com/andrader/scaffold/actions/workflows/main.yml/badge.svg)](https://github.com/andrader/scaffold/actions/workflows/main.yml)

# Scaffold for Python Project with Continuous Intregation

This is a project scaffold for Python Project with Continuous Intregation.

## Step by step to recreate this repo

### Setting up the enviroment

- Configure ssh key in your enviroment (AWS, GCP, Azure) shell:
  1. generate ssh key with `ssh-keygen -t rsa` and `enter` `enter` `enter`
  1. print the public key `cat path/to/public/key` and copy it
  1. go to github.com -> setting -> ssh -> add ssh key -> paste your public key -> save it

- Configure git name and email
  1. git config --global user.name "name"
  1. git config --global user.email "email@email.com"

- Create a Python virtual enviroment:
  1. Go to your home `cd ~/`
  1. Crete the virtual enviroment with `python3 -m venv ~/.<YOUR_REPO_NAME>`
  2. Activate the virtual enviroment with `source .<YOUR_REPO_NAME/bin/activate`

### Setting up the repository

1. Create a github repository with name, description, add readme, add .gitignore for python project
2. Go to the new repository page, click Code, click SSH and copy the SSH url
3. In your enviroment shell, clone the repository locally with `git clone <PASTE_SSH_URL>`

5. Create Makefile with build instructions: `touch Makefile` and write it (look at this [Makefile](https://github.com/andrader/scaffold/blob/main/Makefile) for inspiration)
6. Create requirements.txt: `touch requirements.txt` and write it (look at this [requirements.txt](https://github.com/andrader/scaffold/blob/main/requirements.txt) for inspiration)
9. Write your python code: \*.py files
10. Write tests for your code: test_\*.py
11. Run your Makefile instruction locally: `make [Makefilecommand]` (for example `make all`)
12. Save and publish your work: `git add .*`, `git commit -m "message"` and `git push`

### Creating a Github Action

1. In the repository page, go to *Actions*
2. Click on *New workflow*
3. write the workflow as this [main.yml](https://github.com/andrader/scaffold/blob/main/.github/workflows/main.yml)
4. Commit your changes
5. Your should see the Action running in the *Actions* page.
6. Optionally, to see the status of the action in your repository first page: add a badge to the README.md file by going to your repository's Actions page, select your workflow in the left side, click in the three dots in the right side, select *Create status badge* and copy the text. Then edit the README.md, paste the text there and commit changes.


## Duplicating this repository

[Duplicating this repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/duplicating-a-repository)

