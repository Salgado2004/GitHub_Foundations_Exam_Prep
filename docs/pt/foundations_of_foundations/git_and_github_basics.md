# Domain 1: Git and GitHub basics
**Exam weight: 22%**
### Git and GitHub Basics
- **Describe version control**:
  
	Version control is a development practice that allows multiple collaborators to work in the same project. It's designed to track yours and other people's changes or revisions in the same project.
- **Define distributed version control**:
  
	It's the possibility to work with copies of the same project in different places and keep all those copies up to date. 🔁
	
	_Keywords_: `Remote`; `Local`; `Sync`.
- **Describe git**:
  
	It's a Distributed Version Control System (created in 2005 by the Man Himself, Linus Torvalds) and it is the most used of its kind. It's fast, versatile and highly scalable.

	_Reference_: [About git](https://docs.github.com/en/get-started/start-your-journey/about-github-and-git#about-git)
- **Describe GitHub**:
  
	GitHub is a cloud-based platform that uses Git as its core technology and adds features that make collaboration and code management easier. It has a lot of offerings, like showcasing your work, manage changes and review your code.

	_Reference_: [About GitHub](https://docs.github.com/en/get-started/start-your-journey/about-github-and-git#about-github)
- **Explain the difference between Git and GitHub**:
  
	Important❗Git and GitHub are _different_ concepts
	Git is the tool for version control and revision tracking of yout code and managing source code history used generally in a command-line interface. GitHub is a cloud platform that allows Git-related actions accessed via web interface for online collaboration and project management.

	_Reference_: [How do Git and GitHub work together?](https://docs.github.com/en/get-started/start-your-journey/about-github-and-git#how-do-git-and-github-work-together)
- **Describe a GitHub repository**:
  
	It's a place where you can store your code, your files, and each file's revision history. You can view tags, different branches. You can pin it, star it, fork it, and clone it. Basically where you centralize the projects management.
- **Decribe a commit**:
  
	It's a registry of the code in a specific moment in the repository history. ✔️ Represent incremental changes to a codebase. _Not the whole file_. Uses SHA Hashing. 
	
	_Keywords_: `Snapshot`; `Checkpoint`. 
- **Describe branching**:
  
	It's the feature of Git that allows multiple collaborators to work in the same code without its modifications affecting the main branch or overriding each other. It works like alternate timelines of the repo. When the work is done, you can merge different branches.
	
	_Keywords_: `Series of linked commits`; `Tree`; `Reference`.
	_Reference_: [Branching](https://docs.github.com/en/get-started/start-your-journey/hello-world#step-2-create-a-branch)
- **Define a remote in Git terminology**:
  
	Remote is a reference to a remote location where a copy of the repository is hosted (Like GitHub). You can have multiple remote entries. Also called "origin". It uses the concepts of upstream and downstream.

	_Reference_: [About remote repositories](https://docs.github.com/en/get-started/git-basics/about-remote-repositories)
- **Describe the GitHub flow**:
  
	GitHub Flow is the art of working with different branches in the same repository. Creating specific branches for features, bugs, etc. The management of the code in the main branch. Branch-based workflow.

	_Reference_: [GitHub Flow](https://docs.github.com/en/get-started/using-github/github-flow)
### GitHub Entities
- **Describe different GitHub accounts (personal, organization, enterprise)**:
  
	We have three different GitHub accounts:
	- _Personal_ 👤: Basically, every person who uses github.com (normal users)
	- _Organization_ 👥 : It's a shared account where multiple users can have roles, manage and collaborate
	- _Enterprise_ 🏢 : Allow administrators to centrally manage policies and billing for multiple organizations and users
	
	_Reference_: [Types of GitHub Accounts](https://docs.github.com/en/get-started/learning-about-github/types-of-github-accounts)
- **Describe GitHub's products for personal accounts (free, pro)**:
  
	- _Personal free_: Community support, dependabot alerts, deployment protection for public repos, MFA, 500MB packages, 15GB codespaces, 120 hours codespaces, 2000 minutes for actions.
	- _Personal pro_: Everything from free and GitHub support via email, 3000 minutes for actions, 180 hours codespaces, 2GB packages, Advanced tools for private repos, wikis.
- **Describe GitHub's products for organization accounts (free for organizations, teams)**:
  
	- _Free for organizations_: Teams access control, 2000 action minutes, 500MB packages. Everything from personal free.
	- _Teams_: 2GB packages, 3000 action minutes, wikis, scheduled reminders, code owners, draft pull requests, protected branches, repository insights graphic. Everything from free.
- **Describe the different deployment options for GitHub Enterprise**:
  
	There are two different deployment options for GitHub Enterprise:
	- _GitHub Enterprise Cloud_: A set of advanced features on GitHub.com, GitHub support, SAML SSO, security, compliance, deployment protection rules. 50.000 action minutes, 5GB packages, SLA 99,9%. EMU (Enterprise Managed Users) 
	- _GitHub Enterprise Server_: Self-hosted platform that runs on the company's infrastructure. GitHub support. SAML SSO, security, compliance, deployment protection rules. You can use `GitHub Connect` to access some cloud only offerings.

	_Reference_: [GitHub's Plans](https://docs.github.com/en/get-started/learning-about-github/githubs-plans)
- **Describe the features in the user profile (metadata, achievements, profile readme, repositories, pinned repositories, stars, etc)**:
  
	Picture and BIO. Contributions graph (commits, prs, issues, reviews) over the last year. Followers, following. Stars ⭐. Profile readme (it must be in a repo with the same name of your user). Pinned repos (to showcase your profile). Achievements (earned by accomplishing "missions").

	_Reference:_ [Customizing your profile](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/personalizing-your-profile)
### GitHub Markdown
- **Identify the text formatting toolbar on issue and pull request comments**:
  
	It's a feature of github.com to help creating markdown like formatting without the need to know markdown syntax. Also, allows GitHub Flavored Markdown.

  ![image](https://github.com/user-attachments/assets/ce6d183e-13a2-4c37-9573-5ec93582f34e)

- **Describe Markdown**:
  
	A markup language that provides a shorthand syntax to format information. Easy to use. Being readable in its raw format. It also can be used with HTML.

	_Reference_: [Quickstart for writing in GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)
- **Identify the basic formatting syntax (headings, links, task lists, comments, etc)**
	```markdown
	# H1,
	## H2
	**bold**, __bold__
	_italics_, *italics*
	> blockquote
	`code line`
	``` code block ```
	```

- **Explain where to find and use slash commands**:
  
	They are used to help creating complex markdown. "Convenience features". It appears as a prompt when you type slash ("/")

  ![image](https://github.com/user-attachments/assets/6053d9c1-972e-41df-afdd-1faef0b29dbb)


	_Reference_: [About slash commands](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/about-slash-commands)
### GitHub Desktop
- **Explain the differences between GitHub Desktop and github.com**:
  
	github.com is the web interface and main channel to interact with GitHub. GitHub Desktop is a standalone application, and common git and github operations can be performed via the GUI. It's good for starters, but it has much less features.
- **Describe the available features with GitHub Desktop**:
  
	It helps cloning your repos, tracking changes, staging, and commiting your work and managing branches. Managing repos locally. Simplified interface. Limited to local git tools.

	_Reference:_ [About GitHub Desktop](https://docs.github.com/en/desktop/overview/about-github-desktop)
### GitHub Mobile
- **Describe the available features with GitHub Mobile**:
  
	Mobile application to perform basic GitHub repo management tasks. Manage triage and clear notifications. Read, review, and collaborate on issues and prs. Search for repos. Use as MFA secure method. Use GitHub Copilot Chat to ask and receive answers to coding-related questions.
- **Explain how to manage notifications through the GitHub Mobile app**:
  
	You can set push notifications by what you want to receive: Like mentions, reviews, deployments, workflow runs. You can set working hours. Can set swipe options to automatically manage the notifications.

	_Reference_: [About GitHub Mobile](https://docs.github.com/en/get-started/using-github/github-mobile)
