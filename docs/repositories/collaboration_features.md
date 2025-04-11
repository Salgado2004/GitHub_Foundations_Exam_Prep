# Domain 3: Collaboration Features
**Exam weight 30%**
### Issues
- **Describe how to link a PR to an issue**:
	
	You can do manually from either the issue or PR view or you can reference the issue number in the PR description using keywords like "close #8"
	> The keywords are only interpreted when the pull request targets the repo's default branch

  ![Example of issue linking in a PR description](https://github.com/user-attachments/assets/67d74b21-daf2-454c-8fb2-f2709a7940d3)
	
	_Reference_: [Linking a issue to a PR](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue)
	
- **Describe how to create an issue**:
	
	There are several ways to create issues in GitHub, you can use the issue tab, GitHub CLI, from a comment in a thread, from a Discussion, from code files, from GitHub Projects, and now even Copilot! (Though it needs an extension to work). In general, you only needs to provide a Title and Description.

	_Reference_: [Creating an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/creating-an-issue)
	
- **Describe the differences between an issue, discussion, and pull request**:
	
	- _Issue_: Tracking tasks, bugs, enhancements, and other actionable items
	- _Pull request_: Proposing, reviewing, and merging code changes. Directly linked to code changes. Can be linked to issues.
	- _Discussion_: Facilitating conversations and Q&As about a wide range of topics related to the project. Can be "converted" to an issue. Not directly related to code changes.
	
- **Explain how to create a branch from an issue**:
	
	You can create directly in the issue view, in the Development section.

  ![Showing the create link in the development section of the Issue view](https://github.com/user-attachments/assets/db561f12-355c-4900-bae6-b8c92554e808)

	_Reference_: [Creating a branch from an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/creating-a-branch-for-an-issue)
	
- **Identify how to assign issues**: 
	
	You can do it directly in the issue view, by selecting the assignees.

  ![Assigning dropdown in the Assignees section of the Issue View](https://github.com/user-attachments/assets/a6155375-e32c-42d4-9625-fcac84fe3f77)

	_Reference_: [Assigning issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/assigning-issues-and-pull-requests-to-other-github-users)
	
- **Describe how to search and filter issues**:
	
	Sort through lots of issues. You can use the UI or the query language of GitHub (based on keywords like `is:issue`, `author:username` and using boolean operators like AND/OR)

	_Reference_: [Filtering and searching](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/filtering-and-searching-issues-and-pull-requests)
	
- **Describe how to pin an issue**:
	
	You can pin the issues just like the repos, and they will appear in the top of the issues list. You can pin up to three issues. 

	_Reference_: [Pinning an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/administering-issues/pinning-an-issue-to-your-repository)
	
- **Explain basic issue management**:
	
	You can add labels, associate it with a milestone, can create a branch or associate one to mark the development of the issue. Can automatically close it with a PR. Assign a contributor to be responsible for the issue. Add it to a project. Set notifications. 

	_Reference_: [About Issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)
	
- **Explain the difference between issue templates and issue forms**:
	
	- _Issue templates_: Markdown templates pre-loaded when creating a new issue
	- _Issue forms_: (beta) YAML file to declare a form like interface (with input boxes) to create a new issue

   ![Example of issue form](https://github.com/user-attachments/assets/b9181ff7-eddc-471e-9c62-5bb883f5a261)
	
	_Reference_: [Issue templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates#issue-templates)
	
- **Explain how to use keywords in issues**:
	
	These keywords can be used to link issues to pull requests or mark them as duplicated. To mark as duplicated you just type "duplicate of" and them reference the source issue.

	_Reference_: [Marking issues as duplicates](https://docs.github.com/en/issues/tracking-your-work-with-issues/administering-issues/marking-issues-or-pull-requests-as-a-duplicate)
### Pull requests
- **Describe a pull request**:
	
	A feature for proposing, reviewing, and merging code changes. Directly linked to code changes. Can be linked to issues. "A formal process to merge changes". Provides collaborative reviews, automated testing, controlled integration.

	_Reference_: [About Pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests#about-pull-requests)
	
- **Explain how to create a new pull request**:
	
	You can create it via CLI or web interface. You must choose the `base` branch and the `compare` branch (also called `head`). The title and description are not required but are recommended.

	_Reference_: [Creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
	
- **Describe the _base_ and _compare_ branches in a pull request**:
	
	The compare branch is the branch with changes you want to include, your "source". The base branch is the branch you want to push your changes to, your "target". You can have compare branches across forks.
	
- **Explain the relationship of commits on a pull request**:
	
	Create a merge commit, squash and merge, rebase and merge
	
- **Describe draft pull requests**:
	
	It's a feature available only for the Organizations plan (and beyond) that allows to open the pull request but mark it as work-in-progress (WIP). It communicates that the pull request is not ready to be merged and ensures incomplete work is not accidentally merged. Is a feature only for Teams. Cannot be merged nor reviewed.

	_Reference_: [Draft pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests#draft-pull-requests)
	
- **Describe the purpose of the pull request tabs (conversation, commits, checks, files changed)**: 
	
	The conversation tab has the history of the pull request and all the activity. Commit tab has all the commits in the compare branch that are going to be included in the base branch. Checks tab include checks that can be created with actions (unit tests, code quality). Files changed tab includes a summary of the additions and deletions in the pull request per file. 
	
- **Identify how to link activity within a pull request**:
	
	You can do it manually from the issue or pr view, or automatically using the supported keywords (close, closes, fix, fixes, resolve, resolves). They call it "issue linking"
	
- **Explain the different pull request statuses**:
	
	Open, draft, closed (withoud merging), merged, changes requested, review required (needs a review before being able to merge), approved (can be merged), conflict, ready for review (comes after draft). 
	
- **Recognize how to comment on a posted link to a line or lines of code from a file**:
	
	You can do this going to the Files changed tab, and opening the dialog option in the editor by clicking in the desired change.

	_Reference_: [Commenting on a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/commenting-on-a-pull-request)
	
- **Describe code review with a codeowners file**:
	
	The codeowners file is used to assign a collaborator as "responsible" for some part of the code. When you create a pull request that changes this part of the code, it automatically requests the review from the codeowner.

  ![Activity from a Pull Request where dependabot required my review as a codeowner](https://github.com/user-attachments/assets/c3915ec0-eb26-4010-a065-ad59b511c4de)

	_Reference_: [About codeowners](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners)
	
- **Explain the different options for providing a code review on a pull request (comment, approve, request changes, suggested changes)**:
	
	Every review for a pull request is a comment, but you can add extra context (such as approve or request/suggest changes). You can create branch protection rules like "require approval" to allow merging the pull request.

  ![Review form with options 'Comment', 'Approve' and 'Request changes'](https://github.com/user-attachments/assets/7dd2261c-f050-4e07-948c-344c7e70077e)

	_Reference_: [Reviewing pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews)
### Discussions
- **Describe the difference between issues and discussions**:
	
	GitHub Discussions is a communication tool that supports threaded conversation, categorization, community interaction about a wide range of topics related to the project. Can be "converted" to an issue (I say it with commas because in reality you just mention the discussion in the issue description). They are not directly related to code changes.

	_Reference_: [About Discussions](https://docs.github.com/en/discussions/collaborating-with-your-community-using-discussions/about-discussions)
	
- **Explain the options available with discussions (announcements, ideas, polls, Q&A, show and tell)**: 
	
	You can create your own categories. When you create a new category, you can set the discussion format (Announcement, poll, open-ended conversation, question/answer).

  ![Categories in the GitHub Community](https://github.com/user-attachments/assets/f9cc52d7-ef69-437f-9324-159d1eb96ba5)

	_Reference_: [Managing discussion categories](https://docs.github.com/en/discussions/managing-discussions-for-your-community/managing-categories-for-discussions)
	
- **Identify how to mark a comment as an answer to a discussion**:
	
	The repo maintainer (or the one who asked the question) can select the answer in the discussion he believes is the most suitable for the problem, to help others find the solution. It's like StackOverflow.

	_Reference_: [Marking a comment as answer](https://docs.github.com/en/discussions/collaborating-with-your-community-using-discussions/participating-in-a-discussion#marking-a-comment-as-an-answer)
	
- **Explain how to convert a discussion to an issue**:
	
	They say convert, but basically you will create a new issue from the discussion. It will prefill the issue title and place the discussion link in the description.

	_Reference_: [Convert a discussion to an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/creating-an-issue#creating-an-issue-from-discussion)
	
- **Recognize how to pin a discussion**:
	
	In the discussion view you can pin it and it will appear on the top of the page. it's good to highlight some relevant discussions in your repo.

  ![Pinned discussions in the GitHub Community](https://github.com/user-attachments/assets/7a91fd50-65c7-487d-b3ac-6f433e1fb261)

	_Reference_: [Pinning a discussion](https://docs.github.com/en/discussions/managing-discussions-for-your-community/managing-discussions#pinning-a-discussion)
### Notifications
- **Describe how to manage notification subscriptions**:
	
	You can find it in yout profile settings. You can manage your notifications email. You can manage where you will be notified (email, GitHub, CLI) for each subscription.

	_Reference_: [About notifications](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/creating-an-issue#creating-an-issue-from-discussion)
	
- **Explain how to subscribe to notification threads**:
	
	In the thread, you can check to subscribe manually, but you're also automatically subscribed when you  write a comment or you are mentioned in a comment in the thread.
	
- **Describe how to find threads where you are at-mentioned**:
	
	You can filter using keywords, specifically `reason:mention`

	_Reference_: [Reasons for receiving notifications](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/setting-up-notifications/about-notifications#reasons-for-receiving-notifications)
	
- **Identify the notification filtering options**:
	
	They use similar keyword to filtering issues and prs (author, repo, is, org and reason)

  ![Notifications filtering view](https://github.com/user-attachments/assets/2773d00a-0891-41ec-ae07-5c3a982eef6a)

	_Reference_: [Managing notifications](https://docs.github.com/en/account-and-profile/managing-subscriptions-and-notifications-on-github/viewing-and-triaging-notifications/managing-notifications-from-your-inbox)
	
- **Explain the different notification configuration options**:
	
	You can choose the type of activity you want to receive. You can choose the channel of notification (web interface, mobile, e-mail). You can make custom notifications for specific repos.
### Gists, Wikis, and GitHub Pages
- **Explain how to create a GitHub gist**:
	
	Gists provide a simple way to share code snippets with others. Every gist is a repository of one file. They can be public or secret (secret is **not** private). You can pin gists in your profile. Can be changed to public. Cannot be changed to private. Allow users to comment.
	To create one is simple, you can add a name, file extension and content.

	_Reference_: [About gists](https://docs.github.com/en/get-started/writing-on-github/editing-and-sharing-content-with-gists/creating-gists#about-gists)
	
- **Describe how to fork and clone a gist**:
	
	They work like a regular repo. But you can also embed in your website
	
- **Explain GitHub Wiki pages**:
	
	Wiki is a repository feature for hosting documentation with multiple nested pages. Serve as knowledge base for the repo. Can use other forms of markup languages, not only markdown.

	_Reference_: [About wikis](https://docs.github.com/en/communities/documenting-your-project-with-wikis/about-wikis)
	
- **Describe how to create, edit and delete wiki pages**:
	
	It can be done using different markup languages
	
- **Explain the visibility of wiki pages**:
	
	They are tied to the repo visibility. If the repo is public the wiki is public.
	
- **Describe GitHub Pages**:
	
	Allow to deploy and host static websites via GitHub repository. You can deploy from a branch or using GitHub Actions. Originally, the repo had to be named as your user, but now it can be named anything. Personal free accounts can only deploy public repos. If you own a public domain, you can use it here.

  ![Deployment to GitHub pages view](https://github.com/user-attachments/assets/dc672021-6077-4f4b-8cce-d7daa7cf3406)

	_Reference_: [About GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)
