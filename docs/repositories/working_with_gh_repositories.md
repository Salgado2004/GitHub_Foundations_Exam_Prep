# Domain 2: Working with GitHub Repositories
**Exam weight: 8%**
### Understading GitHub Repositories
- **Describe the components of a good README and the recommended repository files (LICENSE, CONTRIBUTING, CODEOWNERS)**:

	`READMEs` are markdown files in the project root rendered in the first page of the repo. They provide context and documentation. It's most likely the first thing a visitor will notice in your repository and typically includes information like: What the project does, why the project is useful, how users can get started with the project, and more.
	Other recommended repository files are: 
	- The `LICENSE`, to provide information about code property. 
	- `CONTRIBUTING`, to provide information about how to contribute if it's an open-source project. 
	- `CODEOWNERS`, used to set specific contributors as "responsible" for some part of the code.

	_Reference_: [About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes), [Customizing your repo](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository)
	
- **Explain basic repository navigation**:

	You can navigate between the different tabs of the repository: Code, Issues, PRs, Actions, Projects, Wiki, Security, Discussions, Insights, Settings.

	The default tab is code and it's where you actually store your project files and can see the history changes, but each tab has it's own purpose that can be really useful in the software development lifecycle.

	_Reference_: [About collaboration](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories#about-collaboration)

- **Explain how to create a new repository**:

	To create a local repo, you can run "git init" in your projects folder and then publish it to GitHub. Or directly in GitHub you can create it in your profile page or with the GitHub CLI. When creating you can pre-set if it's public or private, and if it has README, .gitignore and LICENSE files.

	_Reference_: [Quickstart for repositories](https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories)

- **Describe repository templates**:

	You can turn an existing repo into a repo template or create a new repo from the repo template as a starting point. The difference from the fork, is that it doesn't include commit history, just the files.

  ![image](https://github.com/user-attachments/assets/c31b7a6e-bc31-407a-9a7a-aaf519ceb09c)

	_Reference_: [Template repositories](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-template-repository)

- **Describe the different features to maintaining a repository**:

	Change the default branch. Choose the features (issues, wikis, discussions). Danger zone: change visibility, transfer ownership. archive repo and delete the repo.

  ![image](https://github.com/user-attachments/assets/39212922-4ce1-4c2e-9e64-082848c4c9d5)

- **Describe how to clone a repository**:

	You can clone a repository in three different ways: https, ssh, or GitHub CLI. You can also download the ZIP, but that's **NOT** cloning.

  ![image](https://github.com/user-attachments/assets/065d7507-3142-4e97-87e8-223c6ccde6a5)


	_Reference_: [Cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)

- **Describe how to create a new branch**:

	- _Using GIT_: `git checkout -b <name>`, `git branch <name>`, `git switch -c <name>`
	- _Using GitHub_: Create from issue, directly from UI, using GitHub Desktop 

	_Reference_: [Creating a branch](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository#creating-a-branch)

- **Explain how to add files to a repository**:

	You can create new files directly in the GitHub UI, upload files or use the command line with GIT. 

	_Reference_: [Adding a file to a repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)

- **Identify how to view repository insights**:

	_Note_: Not all of them are available for private repos in the free tier:
	- _Pulse_: Overview of recent activity (issues open/closed, pull requests open/closed), summary of activity, top contributors, list of unresolved conversations
	- _Contributors_: List of contributors and their activity stats.
	- _Community standands_: Checks for essential community health checks
	- _Commits_: History of all commits in the repo
	- _Code frequency_: Graph of code additions and deletions over time
	- _Dependency graph_: Visualize code dependencies
	- _Network_: Show fork relationships and variations (also shows the GitHub Flow for each fork)
	- _Forks_: Number of forks and links to repository forks

	_Reference_: [Viewing activity for your repository](https://docs.github.com/en/repositories/viewing-activity-and-data-for-your-repository)

- **Explain how to save a repository with stars**:

	Stars are used as popularity count. Keep track of the repo. You can see the starred repo in _github.com/stars. You can see who starred a specific repo in _github.com/\<user\>/\<repo\>/stargazers_

	You can organize the repositories you starred in lists, like "Inspiration", "Best practices", etc, to make it easier to find them again.

	_Reference_: [GitHub Stars](https://docs.github.com/en/get-started/exploring-projects-on-github/saving-repositories-with-stars)

- **Explain feature previews**:

	Feature previews is a place in GitHub where you can enable or disable some beta features that are available for testing. Slash commands and Copilot Workspace for pull requests, for example, are in feature preview now (april/2025)

  ![image](https://github.com/user-attachments/assets/30575d4d-ab06-4f5e-85ed-e54e2a215cff)

	_Reference_: [Feature preview](https://docs.github.com/en/get-started/using-github/exploring-early-access-releases-with-feature-preview)
