#GitHub Cheat Sheet

#What is GitHub?
  GitHub is a web host that translates git, and stores files.

#How do I create a repo on GitHub?
  Go to Github.com and click create repository.

#I forked a repo, how do I get it to my computer?
  When you fork a repo, you create a new repo under your username on GitHub. To get a copy on your computer, you will go to YOUR repo and get the url, in the bottom right corner. Then, on your computer in the terminal, navigate to the folder where you want the project and type ‘git clone [repoURL]’ This command will do two things: 1) Create a local copy of the repo, 2) set up the remote origin. This saves you from having to add the remote yourself. Now, work on the file, and commit when you make changes as normal. When your ready to send to GitHub, type ‘git push origin master’ as normal.

#How do I host my website on GitHub?
  GitHub has a nice feature, called GitHub pages, that allows you to host your HTML pages. Once you have a local repo, and a GitHub repo, and your changes are pushed up to GitHub, you are ready to make a new branch.
To make a branch type ‘git checkout -b [branchName]’ Branches are very useful, and are explained later. To get your page hosted on GitHub, you will need ‘git checkout -b gh-pages’ which will create the pages branch. Then, ‘git push origin gh-pages’ will send your new branch to GitHub, and you can find your page at https://[username].github.io/[repoName]

#Why isn’t my GitHub pages working?
  Does your gh-pages branch exist?
  Do you have a file named index.html for GitHub to find, at the root (not inside a folder) of your gh-pages branch?
  Did you verify your e-mail with GitHub?


#What is a pull request (PR)?
  A pull request is a feature of GitHub, that allows changes from one branch to be pulled into another. An example would be on a project with multiple collaborators, where each person works on their own forked copies of a repo. When someone is ready to send their changes to the master repo, a pull request is created. This allows for whoever is controlling the master repo, to review the changes before they are added.

