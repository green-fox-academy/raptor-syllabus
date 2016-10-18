# Module 1: Day 3 - The Command line & Git

## Materials & Resources
Go through these tutorials:

 - https://www.codecademy.com/learn/learn-the-command-line
 - https://www.codecademy.com/learn/learn-git (__Note__ only review the first two sections: "Git Basic Workflow" and "How to Backtrack")
 - https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes
 - Install Git on your system, visit this link:
   - https://github.com/greenfox-velox/velox-syllabus/tree/master/week-01/3-command-line#please-install-git-on-your-system

If you can:
- Proceed to read the next 2 chapters of git and try this link
https://try.github.io/

Any other questions, post them on a Trello card as a comment and in the morning we'll discuss.

## Prepare your machine
- Please install git on your system:
  - Windows (*portable* is good however the *installed* version is better)
    - Ensure you have the command-line, bash version also which you can find at 
    http://cmder.net/ or https://git-scm.com/download/win
  - Linux
    - `sudo apt-get install git` (Ubuntu)
    - `sudo yum install git` (Fedora)
  - Mac
    - http://git-scm.com/download/mac or `brew install git`

## Assignment Review
- `cd`
- `.` and `..`
- `pwd`
- `ls`
- `touch`
- `mkdir`
- `cp`
- `mv`
- `rm`
- command options
- `<` and `>` and `>>` and `|`
- `sort`
- `uniq`
- `grep`
- `sed`
- git `init`, `clone`, `add`, `rm`, `commit`, `push`, `pull`, `remote`

## Workshop/Tasks for this day
  - Try to work without using your mouse; only use it if there's no other way (try to force yourself to learn the control codes; this improves your productivity)
  - Command-line
    - setup the environment
    - basic terminal operations
    - manipulations
    - redirections
    - scripts
  - Git
    - basics
    - workflow
    - getting used to
    - saving all your previous work
    - creating a website yaaay :)

## Tasks in detail

### Command Line Basics
  - Open a terminal (with git ;) )

#### Basic terminal operations
  - Check the current working directory
  - Check the files and directories in your working directory
  - Create a Greenfox directory
  - Change into the Greenfox directory
  - Check the files and directories in your working directory
  - Create an empty index.html file
  - Create an images directory
  - Create a css directory
  - Change into the images directory
  - Go back to the parent directory
  - Create at least one file to every directory

---
  - Fork this git repository: https://github.com/greenfox-velox/velox-syllabus
      - Visit the page
      - Fork it!
  - Clone your greenfox repository
      - `git clone <repository>`
  - Change into week-01/3-command-line/ directory

#### Manipulations
  - Change into the project directory
  - List the detailed file and directory informations
  - Copy the index.html into about.html
  - Create a temp_images directory
  - Copy 1.jpg and 2.jpg into temp_images directory
  - Copy every jpg file into temp_images directory
  - Move 6.jpg file from css into images directory
  - Delete 7.jpg from css directory
  - Navigate up one directory from project/css/ to project/

#### Redirections
  - Echo a string to a file
  - cat a file content and redirect the content to another file
  - redirect a file content to cat command
  - count the words in index.html
  - cat a file content and pipe to wc
  - sort a file
  - sort a file and redirect the input to a file
  - remove the duplicated lines from tasks.txt
  - cat task.txt and filter basic tasks
  - cat task.txt and filter out with -v the basic tasks

### Git

#### Basics
  - setup your environment
  - `git config --global user.name "Your Name"`
  - `git config --global user.email yourname@example.com`

---
  - create a repo on github
      - under greenfox-velox organisation and the repo name should be your github username
  - clone it on your system using command line
  - your working directory should look like this
      - home
          - user (your username if you're using mac or linux, on windows its git env username)
              - .hidden_directories...
              - greenfox
                  - githubusername (this should be the cloned repo, which is named after your github username, so the folder on your computer should be named that way as well)
                      - week-01
                          - day-1
                              - contents created on your first day
                          - day-3
              - other_visible_directories

---
  - change in to your githubusername directory
  - see the changes
  - set to staged
  - commit with a nice understandable commit message
      - it's nice if you can write commit messages to complete the following
      - "If this commit is applied it will..."
      - ...create my working directory for greenfox lessons
      - ...create a new directory for task 1
      - ...
  - change in to your week-01/day-3 directory
  - create 5 directory and 5 file with content
  - see the changes
  - add these files as staged files
  - use git status to check
  - commit it with commit message
  - change the content of two file
  - set to staged
  - use git status
  - commit it with commit message
  - git pull
  - git push origin master
  - check it on github

---
  - change the content of two file
  - use git status
  - remove from staged git reset HEAD file

---
  - change the content of two file
  - use git status
  - set to staged
  - git diff --staged or --cached
  - commit it
  - check it on github

#### Build Habits
*Get used to saving your work!*
  - Save the Command-line edits
    - change back to the directory where you completed the Command-line phase
    - this should be a git repository as well
    - stage and commit the changes, and push it to your remote repo
    - see it on Github
  - From tomorrow you'll only work in one repository found under the greenfox-raptor organisation
    - easier to track everything related to your progress in one repository
    - we won't learn how to create git repositories inside other git repositories, but a link would be nice for today's learning curves ;)
    - create a README.md file in your main greenfox repository root
    - check out how to create a link in Markdown syntax: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links
    - create a link for your cloned syllabus repo with a nice title (stage, commit and push)

#### Creating a website
*The cherry on the cake for today*
Create a new repo under your username at github called yourgithubusername.github.io
  - Make a local version of it (clone)
      - Pay attention not to clone inside another git repo!
  - Create an index.html file with content, images and styling or use the ones from first day
  - push!
  - see your website at http://githubusername.github.io
  - note, this is another repo, so you should include links in your main README.md
      - about the website
      - and the repository as well
