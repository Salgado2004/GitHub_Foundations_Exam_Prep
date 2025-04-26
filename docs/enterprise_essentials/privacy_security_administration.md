# Domain 6: Privacy, Security, and Administration
**Exam weight 10%**
### Authentication and Security
- **Explain how to secure your account with 2FA**:
	
	Multi-factor authentication. Use a secondary device to enter a code as an extra security precaution. There are different methods to choose as 2FA, like authenticator apps (authy, Microsoft authenticator), SMS, security keys, GitHub Mobile, or the recovery codes.

  ![](https://github.com/user-attachments/assets/a0a96106-86cd-4132-b18c-3626cb610e8e)

	_Reference_: [About multi-factor authentication](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/about-two-factor-authentication)
	
- **Describe the different access permissions**:
	
	For personal accounts
	- _Owner_: The person who owns the repository. Cannot be shared. Invite collaborators, danger zone, manage topics, social media preview, create template, basically full control of the repo
	- _Collaborator_: People you add as collaborators. Write and read access. Manage labels and milestones. Manage the code
	For business accounts
	- _Owner_
	- _Billing manager_
	- _Member_
	For enterprise accounts
	- _Owner_
	- _Billing manager_
	- _Member_
	- _Guest collaborator_

	_Reference_: [Access permissions on GitHub](https://docs.github.com/en/enterprise-cloud@latest/get-started/learning-about-github/access-permissions-on-github)
	
- **Explain EMUs (Enterprise Managed Users)**:
	
	Enterprise Managed Users allows you to manage the lifecycle and authentication of the users from an _external Identity Provider_ (Microsoft Entra, OKTA). These IdPs provide SAML authentication and SCIM (System for Cross-domain Identity Management). Azure also provides OCID. Like federations in Azure.

	_Reference_: [About EMUs](https://docs.github.com/en/enterprise-cloud@latest/admin/managing-iam/understanding-iam-for-enterprises/about-enterprise-managed-users)
### GitHub Administration
- **Explain how to enable and disable features**:
	
	You can manage your features in the repository settings. They are in the section features and there are checkboxes to enable or disable them. (Wikis, discussions, issues, sponsorships, preserve this repo, projects)

  ![](https://github.com/user-attachments/assets/904013a2-c811-46ce-a1b6-9cc898bd193d)

	_Reference_: [Enabling features for repositories](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository)

- **Recognize repository permission levels**:
	
	For personal repositories, you have only two permissions levels: owner and collaborator.
	- _Owner_: Full control of the repository (**Cannot be shared**)
	- _Collaborator_: Write access for the repository (pull and push)
	
	_Reference_: [Permission levels for a personal repository](https://docs.github.com/en/enterprise-cloud@latest/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-user-account-settings/permission-levels-for-a-personal-account-repository)

- **Identify the options for repository visibility**:
	
	- _Public_: Anyone on GitHub can find it. It will be on Discover tab.
	- _Private_: Only users with permission can see it. Even with the link, it will give 404 error if someone without access tries to see it. 
	- _Internal_ (Enterprise cloud only): Only users in the organization can read it. Is the default visibility setting for the repos in the enterprise. Except for EMU, any user in the organization can fork the repo.

	_Reference_: [Personal repositories visibility](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/setting-repository-visibility); [About internal repositories](https://docs.github.com/en/enterprise-cloud@latest/repositories/creating-and-managing-repositories/about-repositories#about-internal-repositories)

- **Explain repository privacy setting options (branch protections, codeowners, required reviwers)**:
	
	Branch protection rules are used to manage the development. You can require pull requests before merging, require status checks, require conversation resolution, require signed commits, require linear history, require deployments to succeed, lock branch, and not allow bypassing. With a branch protection rule you can enforce the number of reviewers needed to approve a pull request.

	 ![](https://github.com/user-attachments/assets/6eacd561-c73a-4167-8f64-04a7a1335010)
	
	_Reference_: [Branch protection rules](https://docs.github.com/en/enterprise-cloud@latest/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule)

- **Describe the main features and options in the Security tab**:
	
	- _Security policy_: Markdown of how security vulnerabilities should be reported. 
	- _Dependabot_: Manage and update dependencies for your repo. Alerts due to outdated dependencies. Can create pull requests to update them for you
	- _Code scanning_: CodeQL analysis. Automatically detect code vulnerabilities and code errors
	- _Secret scanning_: Used to protect known secrets that could leak in your repo

	_Reference_: [GitHub Security Features](https://docs.github.com/en/code-security/getting-started/github-security-features)

- **Define repository insights**:
	
	It is a section of the repository with some charts and summaries to provide useful information about the repo and the development

	_Reference_: [Viewing activity for your repository](https://docs.github.com/en/repositories/viewing-activity-and-data-for-your-repository)

- **Explain how to manage collaborators**:
	
	Collaborators are other users who have access to the repository. You can invite them and set the permission level. Can edit permission level and even remove the collaborator access. If the invitation is not accepted by the user in 7 days, it expires.

	_Reference_: [Inviting collaborators](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository)

- **Explain how to manage organization settings**:
	
	You can manage the users in your organization by teams. You can have a visibility for the team. Assign projects or issues for a team. You can manage access to repositories with teams. Can be mentioned in discussions. You can have specific roles to manage your organization

	_Reference_: [Managing your organization](https://docs.github.com/en/enterprise-cloud@latest/enterprise-onboarding/setting-up-organizations-and-teams/managing-your-organizations)

- **Describe members, teams, and roles in a GitHub organization**:
	
	Members are singles users of the organization, teams are groups of users who you can manage access to projects, repos, and more. Roles are the permissions each users have, according to its function in the organization. You can assign roles for individual users or for teams. The default roles are:
	- _Read_: View and clone the repository. Download releases. Comment on issues and pull requests
	- _Triage_: Manage issues and pull requests. Label and assign issues. Close and reopen issues and pull requests.
	- _Write_: Push to repository. All from read and triage
	- _Maintain_: Write permission plus create and publish releases. Configure repository settings for non-sensitive fields.
	- _Admin_: Maintain permission plus full control of the repository

	_Reference_: [Repository roles for organizations](https://docs.github.com/en/enterprise-cloud@latest/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#repository-roles-for-organizations)
