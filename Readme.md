Deze bestanden zijn om te oefenen met GitHub en Visual Studio.
Het duurde even maar nu begin ik het te snappen:
Er wordt een local .git folder aangelegd en die maakt het mogelijk om een handshake te maken met een online GitHub Repository.

In local repository:

Initializing Git

Because we created our file locally, we need to push it to GitHub to store it there. The first step is initializing Git.

Run:
git init

Adding files

With Git initialized, we need to mark the HTML file so that it is included in the next commit. This process is also called staging.

Note: A commit is a snapshot of the history of changes to a file.

Run:
add index.html

This command marks the index.html file so it can be included in the next commit.

Committing files

Our file is now marked and ready for its first commit.

Run:
git commit -m "Add index.html"

Pushing to GitHub

Pushing uploads all your local commits to the remote repository. This makes the changes in your file available to people you are working with. There are two parts to this process:

Creating a repository
Pushing the project
Creating a GitHub repository

In your browser, go to github.com and log in if you haven’t yet. Click the plus sign icon at the top right of the page. Then select New Repository.

Pushing the project to GitHub

Remember, you already have a local repository with one file, and you have committed the changes you made to it. The next step is to push these changes to the newly created GitHub repository.

Paste these commands in your Terminal and press Enter to execute them:
git remote add origin https://github.com/NdagiStanley/new-repository.git
git branch -M `main`
git push -u origin `main`

After running these commands, reload the browser page. Your index.html file is now listed in the online repository.

You can make more updates to the repository by running these commands in order:

git add .
git commit -m "Commit message"
git push origin main

Replace the sample text, Commit message, with a descriptive one of your own. If you are working on a branch other than main, use the name of your branch. You can read more about git branching here.

