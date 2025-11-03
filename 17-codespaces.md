**GitHub Codespaces** - allows to create a customized development environment for your project. You can disconnect and reconnect to an active Codespace without affecting its running processes. You can stop and restart a Codespace without losing the changes that you make to your project.

There are four ways to create a Codespace:
1. From a GitHub template or any template repository
2. From a branch in your repository, for new feature work
3. From an open pull request
4. From a commit in a repository's history

You can create more than one Codespace per repository or even branch. There are limits to the number of Codespaces you can create and run at the same time. When creating a new Codespace each time you work on a project, you should regularly push your changes to ensure that any new commits are on GitHub. When using a long-running Codespace, pull from the repository's default branch each time you start working in Codespace to enable your environment to get the latest commit. 

When creating a GitHub Codespace, four processes occur:
1. VM and storage are assigned to your Codespace
2. Container is created
3. Connection to the Codespace is made
4. Post-creation setup is made

When you connect to a Codespace through the web, AutoSave is automatically enabled. When connected through VS Code, you must enable AutoSave. Your work saves to a VM in the cloud. 

If a Codespace is inactive, the application times out after a period of inactivity and stops running. Default timeout is after 30 minutes of inactivity. Data is kept from the last time your changes were saved. Codespace requires an internet connection. 

You can rebuild your Codespace to implement changes to your dev container configuration. Images from the cache speed-up the rebuild process.

