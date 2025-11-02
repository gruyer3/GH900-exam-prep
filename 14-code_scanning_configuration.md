### Configure frequency

CodeQL analysis workflow can be configured to scan code on a schedule or when specific events occur in a repository. Workflow file can also scan code when someone pushes a change and whenever a pull request is created. 

**Scan on Push**
By default, the CodeQL analysis workflow uses the *on:push* event to trigger a code scan on every push to the default branch of the repository and any protected branch. For code scanning to be triggered on a specific branch, the workflow must exist in that branch. When *on:push* scan returns a result that can be mapped to an open pull request, these alerts appear on a pull request in the same place as other pull requests alerts. 

**Scan on PR**
The default CodeQL analysis workflow uses the *pull_request* event to trigger a code scan on pull requests targeted against the default branch. If a pull request is from a private fork, it's only triggered if you've selected the right option in the repository settings. If *pull_request* trigger is configured to scan the pull request's merge commit rather than the head commit, it produces more efficient and accurate results than scanning the branch head on each push. However, if you use a CI/CD system that can't be configured to trigger on pull requests, you can still use the *on:push* trigger so that code scanning maps the results to open pull requests on the branch and adds the alerts as annotations on a pull request. 

***
### Avoid unnecessary scans of pull requests

Can be configured by specyfing *on:pull_request:paths-ignore* or *on:pull_request:paths* in the code-scanning workflow. For example, if the only changes in a pull request are to files with the file extensions .md or .txt you can use the following *paths-ignore* array.
```
on: 
	push: 
		branches: [main, protected] 
	pull_request: 
		branches: [main] 
		paths-ignore: 
			- '**/*.md' 
			- '**/*.txt'
```

***
### Adjust scanning schedule

By default, the CodeQL analysis workflow scans the code in your repository once a week, at a randomly generated day and time, in addition to the scans triggered by events. To adjust this schedule, edit the *cron* value in the workflow.
```
on: 
	push: 
		branches: [main, protected] 
		pull_request: 
			branches: [main] 
		schedule: 
			- cron: '20 14 * * 1'
```
This workflow scans:
- every push to the default branch and the protected branch
- every pull request to the default branch
- the default branch every Monday at 14:20 UTC

