<h1>git</h1><br>

free<br>
open source<br>
scalable<br>
superfast<br>
local<br>
cheap branching and merging<br>
it is a verion control system<br>

<h2>version control system (vcs)</h2>
keeps track of project and files<br>
all details at one place <br>
wont over ride code<br>
they are of 2 types<br>
centralised and distributed<br>

<h2>centralized</h2>
there is a center server which is the main<br>
all can acesss and push back code<br>
collabrative<br>
good for small projects<br>
backup<br>
synchronization<br>

<h2>distributed</h2>
independent<br>
complete project in machine<br>
mirroring repos<br>
we have local repo which we can push via network connection and can be pulled by someone else<br>
Example- git, mercurick<br>

<h2>github</h2>
web based hosting service<br>
cant use without git<br>
cloud based<br>

<h2>local repository</h2>
working on code, changes and push to repo<br>

<h2>index or working directory and staging area</h2>
format and review code<br>

<h2>push</h2>
send a change to another repo (upload)<br>

<h2>pull</h2>
grab a change from a repo (download)<br>

<h2>clone </h2>
bring a repo copy<br>

<h2>add</h2>
before commit (track files)<br>

<h2>blob (binary large object)</h2>
each file has version represented by blob<br>
holds data and meta data<br>
in git files are not addressed by names but are content addressed<br>

<h2>tree</h2>
it is an object<br>
directory structured<br>
holds blobs and sub directories<br>
maintains association and relationship<br>
binary files holds references of blobs<br>

<h2>in github UI color</h2>
white - no change<br>
green - changed<br>
red - removed<br>

<h2>workflow of git</h2>
 working directory<br>
 |<br>
 (git add)<br>
 |<br>
 staging area <br>
 |<br>
 (git commit)<br>
 |<br>
 repository (change)<br>

<h2> git command line</h2>

<h4>git --version</h4>
for version<br>

<h4>git config --global user.name "Your Name"</h4>
<h4>git config --global user.email "your.email@example.com"</h4>
for linking<br>

<h4>git init</h4>
creates a github repo<br>

<h4>git status</h4>
gives current status<br>

<h4>git commit -m</h4>
-m is for message<br>

<h4>git remote -v</h4>
check<br>

<h4>git remote add origin (link).git</h4>

<h4>git push master origin</h4>
for global<br>

<h2>to clone a repo</h2>
copy url<br>
git clone (url)<br>

<h2>SSH key</h2>
like authentication<br>
to make sure you are the owner<br>
<br>
in terminal<br>
ssh-keygen -t ed25519 -C "your_email@example.com"<br>
name your key<br>
set a passphrase<br>
copy public keyy(.pub)<br>
copy and add the key to github<br>

<h2>github workflow</h2>
write code<br>
|<br>
commit code changes<br>
|<br>
pull request<br>

<h2>local git workflow</h2>
write code<br>
|<br>
stage code changes (git add)<br>
|<br>
commit changes<br>
|<br>
git push<br>

branch 
all commits

master branch
default branch

feature branch
adding major changes/features
takes master branch part and creates a feature branch
feature branch has al commits
master branch has no awarness of feature branch

merging
changes of one branch to another

hotfix branch
for fixing a bug
feature branch is not stable 
so we need to create another branch do changes
and merge back to master

git branch
which branch we are at
* indicates which current branch

  git checkout
  move across  branch

  -b
  to create a new branch
  syntax-
  git checkout -b branch_name
  
