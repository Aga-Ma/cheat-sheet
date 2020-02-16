# Git bash

Simple git bash cheat sheet, based on udemy course [Command Line Essentials: Git Bash for Windows](https://www.udemy.com/course/git-bash/).  
Used as a help for participants of my [git training](https://github.com/Aga-Ma/g4g_git_training)

# Table of contents
- [Git bash](#git-bash)  
- [Table of contents](#table-of-contents)  
- [Where Am I? What's Here?](#where-am-i?-what's-here?)  
- [Working with directories](#working-with-directories)  
  - [Change directory](#change-directory)  
  - [Create & remove](#create-&-remove)  
- [Working with files](#working-with-files)  
  - [Create](#create)  
  - [Rename](#rename)  
  - [Review content](#review-content)
  - [Output to a file](#output-to-a-file)  
  - [Delete](#delete)  

# Where Am I? What's Here?
```bash
pwd
ls
ls -l
ls -la
```

# Working with directories
## Change directory
```bash
cd <dir>
cd .
cd ..
```
## Create & remove
```bash
mkdir dir_name/ #creates <dir_name> directory
rmdir dir_name #deletes empty directory
rm -rf dir_name/ #delete not empty directory
```

# Working with files
## Create
```bash
touch file_name.txt
```
## Rename
```bash
mv file_name.txt file_name-1.txt
```
## Review content
```bash
cat file_name.txt
less file_name.txt
```
## Output to a file
```bash
echo "hello world!" >> file_name.txt
echo "Hi!" > file_name.txt #overwrittes content
```
## Delete
```bash
rm file_name.txt
```
