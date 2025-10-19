### Components of GitHub Flow

***Branches*** are an essential part of the GitHub experience. They let you make changes without affecting the default branch. Your branch is a safe place to experiment with new features or fixes. If you make a mistake, you can revert changes or push more changes to fix the mistake. The changes won't update on the default branch until you merge your branch.

You can create a new branch by using a terminal:
```
git checkout -b new_branch_name
```

***Commit*** is a change to one or more files on a branch. Each commit is tracked by unique ID, timestamp and contributor, regardless of whether it's made via the command line or directly in web interface. 

You can create a commit using a terminal:
```
git commit -m "commit message"
```

Within a git repository, a file can exist in several valid states. The primary states for a file in a Git repository are *Untracked* and *Tracked*.
***Untracked*** - initial state of a file when it isn't yet part of the repository and Git is unaware of its existence.
***Tracked*** - file that is actively monitored by Git. It can be in one of the following substates:
- ***Unmodified*** - file is tracked, but it hasn't been modified since the last commit.
- ***Modified*** - file has been changed since the last commit, but these changes aren't yet staged for the next commit.
- ***Staged*** - file has been modified and the changes have been added to the staging area. These changes are ready to be committed.
- ***Committed*** - the file is in the repository's database. It represents the latest committed version of the file.

***
### Pull requests

***Pull request*** is the mechanism used to signal that the commits from one branch are ready to be merged into another branch. The team member submitting the pull request asks one or more reviewers to verify the code and approve the merge. These reviewers have the opportunity to comment on changes, add their own or use them for further discussion.

***Draft Pull Requests*** are pull requests that are not yet ready for review.

Once the changes have been approved, the pull request's source branch is merged into the base branch.

***
### The GitHub Flow

***The GitHub Flow*** is a simple workflow that helps you safely make and share changes. It's great for trying out ideas and collaborating with your team using branches, pull requests and merges.

1. Create a branch so your changes don't affect the main branch
2. Make updates in the branch. If supported, changes can be deployed from this branch to test before merging.
3. Open pull request to begin a review.
4. Review the comments and make necessary updates.
5. Get approval and merge the pull request into the main branch.
6. Delete the branch to keep repository clean.

***Git Flow Branch types***
- ***master*** - always reflects production-ready code.
- ***develop*** - contains the latest development work for the next release.
- ***feature/**** - used to create new features, branched from develop and merged back when complete.
- ***release/**** - prepares a new production release from develop, allows final testing and minor bug fixes
- ***hotfix**** - quickly patch production issues, branched from master

***Git Flow Process***
1. Feature branch is created to build new functionality
2. Release branch is created to isolate release preparation work so development can continue uninterrupted.
3. Bug fixes may be added to the release branch, but major features should wait for a future release.
4. Release branch is merged into master and tagged with a version number.
5. The same release branch should be merged back into develop to keep it in sync.
6. In case of critical production bugs, a hotfix branch is created from master. Once fixed, it's merged into both master and develop.

***When to use Git Flow***
- For projects with scheduled or versioned releases.
- To maintain multiple production versions.
- For slower, more structured development cycles.




