**Code scanning** uses **CodeQL** to analyze the code in a GitHub repository to find security vulnerabilities and coding errors. It is available for all public repos and for private repos owned by organizations where GitHub Advanced Security is enabled.
If code scanning finds a potential vulnerability or error in your code, GitHub displays an alert in the repository's Security tab. GitHub closes the alert, after the code is fixed. 

***
### Code scanning with CodeQL

**CodeQL** is the code analysis engine GitHub developed to automate security checks. There's three main ways to set it up:
- Default setup - handles choosing the languages to analyze, query suite to run and events that trigger scans with the option to manually configure the languages and query suites. Runs code scanning as a GitHub Actions.
- Advanced setup - add the CodeQL workflow directly to your repository. It generates a customizable workflow file, which uses the *github/codeql-action* to run the CodeQL CLI as a GitHub Actions. 
- CodeQL CLI - may be run directly in an external CI system and uploads results to GitHub

CodeQL supports following languages:
- C or C++
- C#
- Go
- Java/Kotlin
- JavaScript/TypeScript
- Python
- Ruby
- Swift

***

### Billing for Actions

Code scanning uses GitHub Actions and each run of a code-scanning workflow consumes minutes for it. 
GitHub Actions usage is free for both public repositories and self-hosted runners.