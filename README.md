[![Python application](https://github.com/andrader/scaffold/actions/workflows/main.yml/badge.svg)](https://github.com/andrader/scaffold/actions/workflows/main.yml)

# scaffold
This is a project scaffold for Python

## Requirements
- configure ssh key
  1. ssh-keygen -t rsa
  1. enter enter enter
  1. cat path/to/public/key
  1. copy public key
  1. github->setting->ssh->add ssh key

- configure git name and email
  1. git config --global user.name "name"
  1. git config --global user.email "email@email.com"
 
## Step by step
1. Create a github repository
  name, description, add readme, add .gitignore for python project
2. git clone ssh+github.com/repo
3. touch Makefile, requirements.txt, file.py, test_file.py
4. write Makefile
5. write requirements.txt
6. run make all
7. git add, commit and push
