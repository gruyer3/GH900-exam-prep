***GitHub*** is a cloud-based platform that uses Git, a distributed version control system, as its core. It simplifies the process of collaborating on projects.

***GitHub Enterprise*** platform enhances collaboration through AI-powered pull requests and issues, productivity through Copilot and security by providing quicker feedback to improve security.

Productivity is accelerated with automation that the ***GitHub Enterprise*** platform provides. With built-in CI/CD tools directly integrated into the development process, it lets users automate repetitive tasks and speed up daily work. 

***GitHub Enterprise*** includes native, first-party features like ***CodeQL***, ***secret scanning***, ***Dependabot*** and ***security overview*** to minimize risks. Code remains private while still benefiting from integrated security checks.

***
### Repositories

***Repository*** contains all of your project's files and each file's revision history. It's one of the essential parts that help you collaborate with people. You can use repositories to manage your work, track changes, store revision history and work with others.

***Public repositories*** are accessible to everyone on the internet.
***Private repositories*** are only accessible to you, people you explicitly share access with and for organization repositories, certain organization members.

Cloning a repository allows you to create a local copy of a repository on your computer which is useful for making changes locally and syncing them back to the remote repository.
To clone a repository, use following command:
```
git clone <repository-url>
```
Once the cloning process is complete, navigate into the repository folder:
```
cd <repository-name>
```

***
### Gists

***Gists*** are a feature of GitHub that allows users to share code snippets, notes or other small pieces of information in a lightweight and convenient way. They are mini Git repositories, which means you can fork, clone and version-control them just like a regular repository. They are useful for sharing quick solutions, configuration files or examples without the need to create a full repository.

***Gists features:***
- ***Public and Secret Gists***:
	- ***Public Gists*** - these are visible to everyone and can be discovered through GitHub's search functionality. Ideal for sharing code snippets or solutions that you want to make available to the broader community.
	- ***Secret Gists*** - not searchable or publicly listed but they are not entirely private. Anyone with the URL can access them. Useful for sharing code with a limited audience.
- ***Version control***:
	- Every change made to a gist is tracked, allowing to view the history of edits. This makes it easy to revert to a previous version or see how the snippet has evolved over time.
- ***Forking and cloning***:
	- Allows others to build upon your work or adapt it to their needs.
- ***Embedding***:
	- Gists can be embedded into websites or blogs, making them a great tool for sharing code examples in tutorials or documentation.
- ***Markdown support***:
	- Gists support Markdown formatting, which means they can include rich text, headings, links or images.
- ***Collaboration:***
	- Gists can be shared and collaborated on by multiple users. Forking and commenting on gists enable lightweight collaboration.

***Gists use cases:***
- Sharing quick code examples or solutions.
- Storing configuration files or scripts for personal use.
- Creating templates for commonly used code patterns.
- Sharing error logs or debugging information with others.
- Embedding code snippets in blogs, forums or documentation.

***IMPORTANT!***
Never use gists to store sensitive or confidential data - even in scripts or config files.
***Gists are not fully private***: even secret gists can be accessed by anyone with the link.

***
### Wikis

Every repository on GitHub comes equipped with a section for hosting documentation, called a wiki which can be used to share long-form content about your projects, such as how to use it, how it was designed or its core principles.
If your repository is private, only people who have at least read access to your repository will have access to your wiki.

***
### Feature previews

***Feature Previews*** allow you to try out experimental features before they are officially released. They give you early access to new functionality and allow you to provide feedback to help shape the final product.