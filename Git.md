# GIT CONCEPTS & QUESTIONS

###  :chart_with_upwards_trend: <span style="color: aqua">What is GIT?</span>
GIT is a distributed version control system and source code management (SCM) system with an emphasis to handle small and large projects with speed and efficiency.

###  :chart_with_upwards_trend: <span style="color: aqua">What is a repository in GIT?</span>
A repository contains a directory named .git, where git keeps all of its metadata for the repository. The content of the .git directory are private to git.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the command you can use to write a commit message?</span>
The command that is used to write a commit message is “git commit –a”.  The –a on the command line instructs git to commit the new content of all tracked files that have been modified. You can use “git add<file>” before git commit –a if new files need to be committed for the first time.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the difference between GIT and SVN?</span>
The difference between GIT and SVN is

1. Git is less preferred for handling extremely large files or frequently changing binary files while SVN can handle multiple projects stored in the same repository.

2. GIT does not support ‘commits’ across multiple branches or tags.  Subversion allows the creation of folders at any location in the repository layout.

3. Gits are unchangeable, while Subversion allows committers to treat a tag as a branch and to create multiple revisions under a tag root.

###  :chart_with_upwards_trend: <span style="color: aqua">What are the advantages of using GIT?</span>
1. Data redundancy and replication

2. High availability

3. Only one.git directory per repository

4. Superior disk utilization and network performance

5. Collaboration friendly

6. Any sort of projects can use GIT

###  :chart_with_upwards_trend: <span style="color: aqua">What language is used in GIT?</span>
GIT is fast, and ‘C’ language makes this possible by reducing the overhead of runtimes associated with higher languages.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the function of ‘GIT PUSH’ in GIT?</span>
‘GIT PUSH’ updates remote refs along with associated objects.

###  :chart_with_upwards_trend: <span style="color: aqua">Why GIT better than Subversion?</span>
GIT is an open source version control system; it will allow you to run ‘versions’ of a project, which show the changes that were made to the code overtime also it allows you keep the backtrack if necessary and undo those changes.  Multiple developers can checkout, and upload changes and each change can then be attributed to a specific developer.

###  :chart_with_upwards_trend: <span style="color: aqua">What is “Staging Area” or “Index” in GIT? </span>
Before completing the commits, it can be formatted and reviewed in an intermediate area known as ‘Staging Area’ or ‘Index’.

###  :chart_with_upwards_trend: <span style="color: aqua">What is GIT stash?</span>
GIT stash takes the current state of the working directory and index and puts in on the stack for later and gives you back a clean working directory.  So in case if you are in the middle of something and need to jump over to the other job, and at the same time you don’t want to lose your current edits then you can use GIT stash.

###  :chart_with_upwards_trend: <span style="color: aqua">What is GIT stash drop?</span>
When you are done with the stashed item or want to remove it from the list, run the git ‘stash drop’ command.  It will remove the last added stash item by default, and it can also remove a specific item if you include as an argument.

###  :chart_with_upwards_trend: <span style="color: aqua">How will you know in GIT if a branch has been already merged into master?</span>
Git branch—merged lists the branches that have been merged into the current branch

Git branch—-no merged lists the branches that have not been merged

###  :chart_with_upwards_trend: <span style="color: aqua">What is the function of git clone?</span>
The git clone command creates a copy of an existing Git repository.  To get the copy of a central repository, ‘cloning’  is the most common way used by programmers.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the function of ‘git config’?</span>
The ‘git config’ command is a convenient way to set configuration options for your Git installation.  Behavior of a repository, user info, preferences etc. can be defined through this command.

###  :chart_with_upwards_trend: <span style="color: aqua">What does commit object contain?</span>
1.      A set of files, representing the state of a project at a given point of time

2.      Reference to parent commit objects

3.       An SHAI name, a 40 character string that uniquely identifies the commit object.

###  :chart_with_upwards_trend: <span style="color: aqua">How can you create a repository in Git?</span>
In Git, to create a repository, create a directory for the project if it does not exist, and then run command “git init”. By running this command .git directory will be created in the project directory, the directory does not need to be empty.

###  :chart_with_upwards_trend: <span style="color: aqua">What is ‘head’ in git and how many heads can be created in a repository?</span>
A ‘head’ is simply a reference to a commit object. In every repository, there is a default head referred as “Master”.  A repository can contain any number of heads.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the purpose of branching in GIT?</span>
The purpose of branching in GIT is that you can create your own branch and jump between those branches. It will allow you to go to your previous work keeping your recent work intact.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the common branching pattern in GIT?</span>
The common way of creating branch in GIT is to maintain one as “Main“
branch and create another branch to implement new features. This pattern is particularly useful when there are multiple developers working on a single project.

###  :chart_with_upwards_trend: <span style="color: aqua">How can you bring a new feature in the main branch?</span>
To bring a new feature in the main branch, you can use a command “git merge” or “git pull command”.

###  :chart_with_upwards_trend: <span style="color: aqua">What is a ‘conflict’ in git?</span>
A ‘conflict’ arises when the commit that has to be merged has some change in one place, and the current commit also has a change at the same place. Git will not be able to predict which change should take precedence.

###  :chart_with_upwards_trend: <span style="color: aqua">How can conflict in git resolved?</span>
To resolve the conflict in git, edit the files to fix the conflicting changes and then add the resolved files by running “git add” after that to commit the repaired merge,  run “git commit”.  Git remembers that you are in the middle of a merger, so it sets the parents of the commit correctly.

###  :chart_with_upwards_trend: <span style="color: aqua">To delete a branch what is the command that is used?</span>
Once your development branch is merged into the main branch, you don’t need
development branch.  To delete a branch use, the command “git branch –d [head]”.

###  :chart_with_upwards_trend: <span style="color: aqua">What is another option for merging in git?</span>
“Rebasing” is an alternative to merging in git.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the syntax for “Rebasing” in Git?</span>
The syntax used for rebase is “git rebase [new-commit]"

###  :chart_with_upwards_trend: <span style="color: aqua">What is the difference between ‘git remote’ and ‘git clone’?</span>
‘git remote add’  just creates an entry in your git config that specifies a name for a particular URL.  While, ‘git clone’ creates a new git repository by copying and existing one located at the URI.

###  :chart_with_upwards_trend: <span style="color: aqua">What is GIT version control?</span>
With the help of GIT version control, you can track the history of a collection of files and includes the functionality to revert the collection of files to another version.  Each version captures a snapshot of the file system at a certain point of time. A collection of files and their complete history are stored in a repository.

###  :chart_with_upwards_trend: <span style="color: aqua">Mention some of the best graphical GIT client for LINUX?</span>
Some of the best GIT client for LINUX is

1. Git Cola
2. Git-g
3. Smart git
4. Giggle
5. Git GUI
6. qGit

###  :chart_with_upwards_trend: <span style="color: aqua">What is Subgit? Why to use Subgit?</span>
‘Subgit’ is a tool for a smooth, stress-free SVN to Git migration.  Subgit is a solution for a company -wide migration from SVN to Git that is:
1. It is much better than git-svn
2. No requirement to change the infrastructure that is already placed
3. Allows to use all git and all sub-version features
4. Provides genuine stress –free migration experience.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the function of ‘git diff ’ in git?</span>
‘git diff ’ shows the changes between commits, commit and working tree etc.
What is the function of ‘git diff ’ in git?

###  :chart_with_upwards_trend: <span style="color: aqua">What is ‘git status’ is used for?</span>
As ‘Git Status’ shows you the difference between the working directory and the index, it is helpful in understanding a git more comprehensively.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the difference between the ‘git diff ’and ‘git status’?</span>
‘git diff’ is similar to ‘git status’, but it shows the differences between various commits and also between the working directory and index.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the function of ‘git checkout’ in git?</span>
A ‘git checkout’ command is used to update directories or specific files in your working tree with those from another branch without merging it in the whole branch.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the function of ‘git rm’?</span>
To remove the file from the staging area and also off your disk ‘git rm’ is used.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the function of ‘git stash apply’?</span>
When you want to continue working where you have left your work, ‘git stash apply’ command is used to bring back the saved changes onto the working directory.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the use of ‘git log’?</span>
To find specific commits in your project history- by author, date, content or history ‘git log’ is used.

###  :chart_with_upwards_trend: <span style="color: aqua">What is ‘git add’ is used for?</span>
‘git add’ adds file changes in your existing directory to your index.

###  :chart_with_upwards_trend: <span style="color: aqua">What is the function of ‘git reset’?</span>
The function of ‘Git Reset’ is to reset your index as well as the working directory to the state of your last commit.

###  :chart_with_upwards_trend: <span style="color: aqua">What is git Is-tree?</span>
‘git Is-tree’ represents a tree object including the mode and the name of each item and the SHA-1 value of the blob or the tree.

###  :chart_with_upwards_trend: <span style="color: aqua">How git instaweb is used?</span>
‘Git Instaweb’ automatically directs a web browser and runs webserver with an interface into your local repository.

###  :chart_with_upwards_trend: <span style="color: aqua">What does ‘hooks’ consist of in git?</span>
This directory consists of Shell scripts which are activated after running the corresponding Git commands.  For example, git will try to execute the post-commit script after you run a commit.

###  :chart_with_upwards_trend: <span style="color: aqua">Explain what is commit message?</span>
Commit message is a feature of git which appears when you commit a change. Git provides you a text editor where you can enter the modifications made in commits.

###  :chart_with_upwards_trend: <span style="color: aqua">How can you fix a broken commit?</span>
To fix any broken commit, you will use the command “git commit—amend”. By running this command, you can fix the broken commit message in the editor.

###  :chart_with_upwards_trend: <span style="color: aqua">Why is it advisable to create an additional commit rather than amending an existing commit?</span>
There are couple of reason

1.  The amend operation will destroy the state that was previously saved in a commit.  If it’s just the commit message being changed then that’s not an issue.  But if the contents are being amended then chances of eliminating something important remains more.
2. Abusing “git commit- amend” can cause a small commit to grow and acquire unrelated changes.

###  :chart_with_upwards_trend: <span style="color: aqua">What is ‘bare repository’ in GIT?</span>
To co-ordinate with the distributed development and developers team, especially when you are working on a project from multiple computers ‘Bare Repository’ is used. A bare repository comprises of a version history of your code.

###  :chart_with_upwards_trend: <span style="color: aqua">Name a few Git repository hosting services</span>
- Pikacode
- Visual Studio Online
- GitHub
- GitEnterprise
- SourceForge.net

###  :chart_with_upwards_trend: <span style="color: aqua"></span>

###  :chart_with_upwards_trend: <span style="color: aqua"></span>

###  :chart_with_upwards_trend: <span style="color: aqua"></span>

###  :chart_with_upwards_trend: <span style="color: aqua"></span>