# Domain 4: Modern Development
**Exam weight 13%**
### GitHub Copilot
- **Describe GitHub Copilot**:
	
	It's an 🤖 AI pair-programming tool to improve code development. It provides features like code snippets directly in the IDE, inline chat to ask questions, context menu for test generation, bug-fixing and documentation, etc. It can be used with multiple IDEs via extensions, in github.com, GitHub Mobile and in the CLI.

   _Reference_: [What is GitHub Copilot?](https://docs.github.com/en/copilot/about-github-copilot/what-is-github-copilot)
  
> [!Note]
> It's a really powerful feature with a lot of content to cover 📚. If you want to know more about Copilot in specific, consider following the [GitHub Copilot Exam Prep](https://github.com/orgs/community/discussions/144443)

- **Describe the difference between GitHub Copilot for Individuals and GitHub Copilot for Business (Subscription plans 💵)**: 

	- _Copilot Free_: Provides limited access to selected features of Copilot, like code completion, copilot chat, copilot review, blocks suggestions matching public code.
	- _Copilot for Individuals (Pro)_: $10 per month, ilimited code completions in the IDE, personal accounts, telemetry, blocks suggestions matching public code, pull request summaries, copilot chat skills.
	- _Copilot for Business_: $19 per user per month, organization or enterprise, blocks suggestions matching public code, plugs in the editor, policy management, audit logs, http proxy via custom certificate, exclude specified files.
	- _Copilot for Enterprises_: $39 per user per month, same as Business plus knowledge bases and fine tunning LLMs (limited preview)

	_Reference_: [Subscription plans for GitHub Copilot](https://docs.github.com/en/copilot/about-github-copilot/subscription-plans-for-github-copilot)
- **Explain how to get started using GitHub Copilot**:
	
	First things first, you need to access GitHub Copilot. If you're an individual user with no access through an organization, Copilot Free is automatically enabled. You can also sign for Copilot Pro.
	
	If you're in an organization or enterprise, the owner needs to purchase the subscription for Copilot Business or Enterprise.
	
	After that, install the copilot extension in your IDE (VS Code, Intellij, NeoVim, etc) and explore it using the shortcuts, Copilot chat, prompting via comments in the file, etc. It is a very natural process, but there are strategies to make the best use of it.

	_Reference_: [Best practices for using GitHub Copilot](https://docs.github.com/en/copilot/using-github-copilot/best-practices-for-using-github-copilot)
### GitHub Actions
- **Describe GitHub Actions (basic understading)**:
	
	GitHub Actions is a CI/CD pipeline ⚙️ directly integrated with your GitHub repository. Allows to automate tests, build images, compile static sites, deploy code to servers and more. The workflow scripts are written in YAML and stored in the `.github/workflows/` folder in your repo.

	_Keywords_: `workflow`, `runner`, `job`, `event`, `step`

	_Reference_: [Understanding GitHub Actions](https://docs.github.com/en/actions/about-github-actions/understanding-github-actions)
- **Explain where you can use GitHub Actions within GitHub (general event types)**: 
	
	You can choose among the several trigger events, which are specific activities that starts the workflow. For example, after a **Push** you can run automated tests, build images, compile static sites, deploy code to servers, automatically check a pull request it's **Open** and more. 

	_Reference_: [Trigger events](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows)
- **Explain where you can find existing GitHub Actions**:
	
	When you create a new workflow, there are some templates of your scripts. You can also search in the marketplace 🛒.

	_Keywords_: `reusable`, `composite`

	_Reference_: [Using Workflow Templates](https://docs.github.com/en/actions/writing-workflows/using-workflow-templates), [Using pre-built actions](https://docs.github.com/en/actions/writing-workflows/choosing-what-your-workflow-does/using-pre-written-building-blocks-in-your-workflow)

![image](https://github.com/user-attachments/assets/438260c9-1d61-4320-b488-a23b791e1e39)


### GitHub Codespaces
- **Describe GitHub Codespaces**:
	
	It's a 📦 container-based development environment, hosted in cloud, where you can code and test your application and it's integrated with one repository. It's acessible anywhere and you can build it with all the dependencies to run your application.

	_Keywords_: `CDE`, `Cloud environment`, `Computing power`

	_Reference_: [What are GitHub Codespaces](https://docs.github.com/en/codespaces/about-codespaces/what-are-codespaces)
- **Identify how do to start a GitHub codespace**:
	
	A codespace is associated with a repository. You can create many codespaces per repository, and even per branch, but you have a maximum you can create in your account. When you clone a repo, you can choose to clone with a codespace. If it's the first time, it's going to need to configure the codespace.
- **Describe the codespace lifecycle**:
	
	It starts when you create the codespace and finishes when you delete it. You can pause it if you want. Create, Rebuild, Stop (freezes the state so you can use later), Delete. They have default timeouts of 30 minutes. It "saves" data, but it's important to commit your changes.

	_Reference_: [Understanging the Codespace lifecycle](https://docs.github.com/en/codespaces/about-codespaces/understanding-the-codespace-lifecycle)
- **Describe the different customizations you can personalize with GitHub Codespaces**:
	
	You can change the number of cores, RAM, storage. Manage the code extensions. You can use VS Code configurations and it will persist. VS Code extensions. VS Code theme. Using dotfiles, shell preferences.

	_Reference_: [Personalizing GitHub Codespaces](https://docs.github.com/en/codespaces/setting-your-user-preferences/personalizing-github-codespaces-for-your-account)
- **Recognize how to add and configure dev containers**:
	
	Visual studio code dev containers allow to configure docker containers via Json files. You can use them in codespaces via the `devcontainer.json` file and configure the settings of VS Code in this file. It enables settings like environment variables, mount remote locations, and basically include the dependencies for your project.

  _Reference_: [Adding a dev container configuration](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration)

  _Example_:

```json
{
  "name": "Node.js & TypeScript",
  "image": "mcr.microsoft.com/devcontainers/typescript-node:1-20-bookworm",
  "forwardPorts": [
    3000,
    4200
  ],

  "postCreateCommand": "npm install",
  "customizations": {
	"vscode": {
	  "extensions": [
		"enkia.tokyo-night",
		"pkief.material-icon-theme",
		"github.copilot",
		"github.copilot-chat",
		"angular.ng-template"
	  ]
	}
  }
}
```

- **Identify how to share a deep link to a GitHub codespace**:
	
	A deep link is a link that points to a specific page that allows creating a codespace. Just a way to generate a URL to generate a codespace from a repo. You can create it and share in the code tab of your repo. It generates the link or the html/markdown to embed in the README

	_Reference_: [Quick creation of codespaces](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/setting-up-your-repository/facilitating-quick-creation-and-resumption-of-codespaces)

![image](https://github.com/user-attachments/assets/5e728512-4bfd-4799-8649-98ddd4e42426)

- **Explain how to use the github.dev editor**:
	
	A VS Code like browser editor with no attached compute. It is intended for quick changes and commiting code. It is very limited compared to the codespace. There's a shotcut to open it by pressing `.` with a repository open.

	_Reference_: [About github.dev editor](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor)
- **Explain the differences between the github.dev editor and GitHub Codespace**:
	
	GitHub.dev has no computing power. GitHub Codespaces offer more options for extensions. GitHub.dev is completely free while GitHub Codespaces has a pre-set number of free minutes you can use per month.
