Check that Git is installed with:
```
git --version
```

To configure Git, you must define some global variables: *user.name* and *user.email*. Both are required to make commits:
```
git config --global user.name "<USER_NAME>"
git config --global user.email "<USER_EMAIL>"
```

Check if the changes worked:
```
git config --list
```

***
### Set up Git repository

Start with creating an empty folder:
```
mkdir folder_name
```

Change directory to the project directory:
```
cd folder_name
```

Initialize new repository and set the name of the default branch to *main*:
```
git init --initial-branch=main
```
or use the following command:
```
git init -b main
```

For Git versions before 2.28.0, use:
```
git init
git checkout -b main
```

Show repository status with:
```
git status
```

***
### Get help from Git

Type following command to get help with what you can do with Git:
```
git --help
```