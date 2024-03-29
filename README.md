# Assignment: Gitting dojo

Welcome to Gitland! You were transferred here with your friend to improve your Git skills! It’s not an ordinary coding dojo. Here you have to cooperate with your partner to solve mysteries of Gitland.

This dojo has specific scenario, some task will be done in parallel some of them belongs to exact person. Initially you will work with our own laptop.

Gitland is full of small creatures called gitties. They can be taught new things by reading Python functions uploaded to GitHub. List of things that gitties need to be taught:

* Introducing themselves - _def introduce()_
* Add two numbers - _def add(a, b)_
* Tell a joke - _def joke()_
* Shout - _def shout()_

This time don't focus on the code too much. Gitties are wiser than python interpreter and are able to fix bugs by themselves. This exercise is aimed to teach you version control, not python.

To help gitties follow steps below carefully.

## Section 1 - repository initialization

Decide which person will be a **Person A** and which will be a **Person B**.

**Person A** has to create a new GitHub repository. Only person A does the steps below. Person B should only watch what A is doing.

  1. Create a folder on your computer using terminal. cd into that folder.
  2. [Initialize a git repository](https://git-scm.com/docs/git-init) inside that folder.
  3. Create a _gittie.py_ file inside that folder. (touch gittie.py).
  4. Add this file to git repository and commit it.
  5. Open web browser. Log into GitHub and find a _New repository_ button. Click it!
  6. Fill in repository name, make sure that _Initialize this repository with a README_ is NOT ticked, and then click _Create repository._
  7. Now the new remote repo is created by Github and it shows some hints to start. Look for " _…or push an existing repository from the command line"._
  section and paste those commands into terminal and press enter. What have those commands just done?
  8. Refresh repository website on github. _gittie.py_ file should show up
  9. Now we'll grant acces to this repository to person B. Go to _Settings_ and than to _Collaborators._
  10. Find person B and click _Add collaborator._

Now it's time for **Person B**:

  1. Check your email. You should find a repository invitation. Accept it.
  2. You should be redirected to the repository page. On this page find a _Clone or download_ button. Click it!
  3. Copy the given url addres.
  4. Open terminal. Type _git clone <copied address>_
  5. What has just happened?

### Section 2 - syncing changes

Now both of you have a local copy of your repository. Now you'll learn to sync your changes.

**Person B**:

  1. Open _gittie.py_ in Atom or Visual Studio Code
  2. Implement _introduce_ function, that'll print, "Hello, I'm Gittie!".
  3. Check _git status_ and _git diff._
  4. Add and commit your changes to git repository.
  5. Push your changes to github. _git push origin master_

**Person A**:

  1. Pull changes from github. _git pull origin master._
  2. Check what happened. _git log_
  3. Open _gittie.py_ file.
  4. Both of you should have identical files now.

### Section 3 - auto merging

1. Now it's time to work simultaneously.
2. **Person A** has implement _add_ function and **person B** has to implement _joke_ function. After doing so, each of you has to add, commit and push your changes to github.
3. Who pushed changes first? Was the second person able to push his/her changes successfully?
4. Read the _git_ output carefully. You'll find instructions there how to push it.
5. After both of you have pushed your changes successfully, use _git pull_ again. Check what happened (git log).

### Section 4 - conflicts

1. Now you'll work independently.
2. Both of you have to modify _introduce_ function. Modify this function body so that it's different than your partners.
3. Commit your changes. Try to sync your changes. What happened? Try to [resolve conflict manually](https://help.github.com/articles/resolving-a-merge-conflict-using-the-command-line/).
4. At the end of this exercise you should have identical files on both computers and git log should give the same output.
5. Now think for a while what happened during this exercise. Do you understand all the parts?

### Section 5 - stashing & popping

1. This time you'll try a common scenario - pulling before committing.
2. Both of you have to implement _shout_ function. However, only **person B** has to add, commit and push it. **Person A** does not commit anything now.
3. **Person A** has to try to pull **person's B** changes.
4. Was the pull successful? What's git's output? What's [_git stash_](https://git-scm.com/docs/git-stash)?
5. Try to stash your changes and pull again.
6. Try to pop your changes from stash.
7. Make your working directory clean.
8. What happened during this section? Can you find any real life use case for git stash?
