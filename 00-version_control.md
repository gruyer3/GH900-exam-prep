***Version Control System (VCS)*** - program or set of programs that tracks changes to a collection of files. Allows team members to work on a project at the same time without affecting each others work as well as to easily recall earlier versions of individual files or the entire project.

1. You can see all the changes made to the project, when they were made, and who made them.
2. Include a message with each change to explain the reasoning behind it.
3. Retrieve past versions of the entire project or individual files.
4. Create branches, which allows several different sets of changes to be worked on at the same time, without affecting the main branch. Branches can be merged if you'd like to keep wanted changes.
5. Attach a tag to a version - for example, to mark a new release.

***Distributed Version Control*** - allows for project's complete history to be stored on both the client and on the server. Files can be edited without a network connection, checked locally and synced with the server when a connection becomes available.

### Git terminology

***Working tree*** - set of nested directories and files that contain the project that's being worked on.

***Repository (repo)*** - directory, located at the top level of a working tree, where all the history and project's metadata is kept by Git. A *bare repository* is the one that isn't part of a working tree; it's used for sharing or backup. 

***Hash*** - represents the contents of a file or another object as fixed number of digits. Git uses hashes that are 160 bits long. Git can tell whether a file has changed by hashing its contents and comparing the result to the previous hash.

***Object*** - Git repo contains four types of objects:
- *blob* object contains an ordinary file
- *tree* object represents a directory; contains names, hashes and permissions
- *commit* object represents a specific version of the working tree
- *tag* object is a name attached to a commit

***Commit*** - committing the changes you have made so that others can eventually see them.

***Branch*** - named series of linked commits. The most recent commit on a branch is called the *head*. The default branch is called *main*, or *master* in Git. Branches allow team members to work independently and later merge their changes into default branch. 

***Remote*** - named reference to another Git repository. When you create a repo, Git creates a remote named *origin* that is the default remote for push and pull operations.

***Commands, subcommands, options*** - Git operations are performed by using commands (for example: git push or git pull) where *git* is the command and *push* or *pull* is the subcommand. Subcommand specifies the operation you want to perform. Commands frequently are accompanied by options, which use hyphens (-) or double hyphens (--), for example: *git reset --hard*

### Git and GitHub

***Git*** is a distributed version control system (DVCS) that multiple team members can use to work on a project. It provides a way to work with one or more local branches and then push them to a remote repository.

***GitHub*** is a cloud platform that uses ***Git*** as its core technology. Simplifies the process of collaborating on projects and provides a website, more command line tools and overall flow. ***GitHub*** acts as the remote repository. 

Key features provided by GitHub:
- Issues
- Discussions
- Pull requests
- Notifications
- Labels
- Actions
- Forks
- Projects
