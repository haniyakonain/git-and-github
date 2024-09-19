# git-and-github

git
free
open source
scalable
superfast
local
cheap branching and merging
it is a verion control system

version control system (vcs)
keeps track of project and files
all details at one pace 
wont over ride code
they are of 2 types
centralised and distributed

centralized
there is a center servr which is the main
all can acesss and push back code
collabrative
good for small projects
backup
synchronization

distributed
independent
complete project in machine
mirroring repos
we have local repo which we can push via network connection and can be pulled by someone else
Example- git, mercurick

github
web based hosting service
cant use without git
cloud based

local repository
working on code, changes and push to repo


index or working directory and staging area
format and review code

push
send a change to another repo (upload)

pull
grab a change from a repo (download)

clone 
bring a repo copy

add
before commit (track files)

blob (binary large object)
each file has version represented by blob
holds data and meta data
in git files are not addressed by names but are content addressed

tree
it is an object
directory structured
holds blobs and subdirectories
maintains association and relationship
binary files holds references of blobs

in github UI color
white - no change
green - changed
red - removed

workflow of git
 working directory
 |
 (git add)
 |
 staging area 
 |
 (git commit)
 |
 repository (change)

 git command line

git --version
for version

git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
for linking

git init
creates a github repo

git status
gives current status

git commit -m
-m is for message

git remote -v
check

git remote add origin (link).git

git push master origin
for global

to clone a repo
copy url
git clone (url)

SSH key
like authentication
to make sure you are the owner

in terminal
ssh-keygen -t ed25519 -C "your_email@example.com"
name your key
set a passphrase
copy public keyy(.pub)
copy and add the key to github

github workflow
write code
|
commit code changes
|
pull request

local git workflow
write code
|
stage code changes (git add)
|
commit changes
|
git push
