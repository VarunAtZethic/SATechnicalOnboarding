# Git Version Control System
### How to install and use Git for version control in Zethic projects

## **_Introduction to Git:_**

Git allows developers to keep a historical record of changes made to their codebase, providing a reliable and efficient way to track and manage versions. Key concepts in Git include:

1. ***Repository:*** A repository, or repo, is a collection of files and their entire history. It serves as a centralized hub for collaboration and version control.

2. ***Commit:*** A commit represents a specific set of changes made to the codebase. Each commit is identified by a unique hash and contains information such as the author, timestamp, and commit message.

3. ***Branch:*** A branch is a parallel version of the codebase that allows developers to work on features or bug fixes independently. Branches enable concurrent development and can be merged back into the main codebase.

4. ***Merge:*** Merging combines changes from one branch into another, typically integrating feature branches into the main branch (often called the "master" or "main" branch).

5. ***Pull Request:*** A pull request (PR) is a mechanism for proposing changes from one branch to another. It allows team members to review, discuss, and provide feedback before merging the changes.

6. ***Remote:*** A remote refers to a repository hosted on a server, such as GitHub or GitLab. Developers can push their local changes to a remote repository and pull changes from it to stay up to date with the latest code.

## **_Setting up Git for the project:_**

To start using Git, follow these steps to set it up on your development machine:

1. ***Installation:*** Download and install Git from the official Git website [Git](https://git-scm.com/downloads). Follow the installation instructions for your operating system.

2. ***Configuration:*** After installation, open a terminal or command prompt and configure your Git identity with the following commands:

```
git config --global user.name "Your Name"
git config --global user.email "yourname@example.com"
```
Replace "Your Name" and "yourname@example.com" with your preferred name and email address, respectively.

3. ***Optional:*** Remote Repository: If you plan to collaborate with others or host your code on a remote repository platform like GitHub or GitLab, create a new repository and obtain its URL.

- **Initialize a Repository:** Open a terminal or command prompt in your project's root directory and run the following command to initialize a Git repository:

```
git init
```
- **Add and Commit Changes:** Use the following commands to stage and commit changes:

```
git add <file1> <file2> ...  # Stage specific files
git add .                    # Stage all files
git commit -m "Commit message"
```
Replace <file1>, <file2>, etc., with the names of the files you want to stage. The commit message should be a concise description of the changes.

- **Creating a branch on git:** You will likely create your new branch from the master branch for all new features/bugs/hotfixes/fixes unless specified otherwise.

The steps to create a new branch are:

- Checkout to the base branch that is ‘master’ (or any other if required) ``git checkout master``
- Fetch all latest changes ``git fetch –all``
- Switch the branch to the new branch that you are going to work on ``git switch -c BRANCH_NAME``

1. Writing a Commit Message:
- chore:* -> Any Regular Changes
- fix:* -> Fix of any type
- feat:* -> New Feature
- docs:* -> Documentation
- test:* -> Test cases
- Try:* -> If you are trying something which you might need to revert
- refactor:* -> If you are refactoring the code

Please do mention in the commit if there are any breaking changes like new env variables or package updates/installs.

You can also practice writing the commit descriptions. If there are more than two points to write in the description, split it into commits.

Ref: [DEV](https://dev.to/puritanic/how-are-you-writing-a-commit-message-1ih7)

2. Creating a Pull Request: Create the pull request for the task that you push to the remote (Github / GitLab).

- **Title** -> Task name from Task tracking tool. (Clickup/Jira)
- **Description** ->Description of the task.

Provide the task name and mention any additional steps required to be done pre-deployment or post-deployment like:

1. Migration needed
2. Add the task to the queue/Jobs
3. Any command that is required to run with a description of why it is required
4. Any env variable that is added. etc.


- **Create and Switch Branches:** To create a new branch and switch to it, use the following command:

```
git checkout -b <branch-name>
```
Replace <branch-name> with a meaningful name for your branch.

- **Push and Pull Changes:** If you're working with a remote repository, you can use the following commands to push your local changes and pull updates from the remote:

```
git push origin <branch-name>    # Push changes to the remote
```

### Information on how to create and manage a module, theme, or distribution project hosted:

## **_Documenting Your Project on Git:_**

Effective documentation is crucial for ensuring the long-term maintainability and understandability of a project. Git provides several features and best practices to help developers document their projects efficiently. This section outlines guidelines for documenting your project on Git, including version control for documentation, commit messages, and documentation file organization.

**Version Control for Documentation:**

Version control is not only useful for tracking code changes but also for managing project documentation. By treating your project documentation as code, you can take advantage of Git's version control capabilities. Here are some tips for version controlling your project documentation:

1. ***Create a Documentation Folder:*** Set up a dedicated folder within your project repository to store all documentation files.
2. ***Commit Documentation Changes:*** Treat your documentation files like any other code file in your project. Use `git add` and `git commit` to track changes and commit new versions of your documentation.
3. ***Use Descriptive Commit Messages:*** Write clear and concise commit messages that describe the purpose and content of the documentation changes. This helps other developers understand the intent behind each commit.

**Commit Messages for Documentation:**

Writing informative and meaningful commit messages is essential for maintaining a well-documented project history. Consider the following best practices when writing commit messages for documentation:

1. ***Be Descriptive:*** Clearly describe the purpose of the documentation changes in the commit message. Use present tense and succinctly summarize the modifications.
2. ***Include Relevant Context:*** Provide additional context or references, such as issue numbers or related documentation, in the commit message. This helps others understand the context behind the changes.
3. ***Consider Length and Readability:*** Keep commit messages concise, but ensure they convey enough information. Avoid excessively long messages that may be difficult to read or understand.

**Documentation File Organization**

Organizing your documentation files in a logical and structured manner helps developers navigate and find information easily. Consider the following guidelines for organizing your documentation files:

1. ***Use a Consistent Structure:*** Define a consistent structure for organizing different types of documentation files, such as user guides, API documentation, or project README files. This makes it easier for developers to locate specific information.
2. ***Create Separate Files for Different Topics:*** Split your documentation into separate files for different topics or sections. For example, have separate files for installation instructions, configuration, usage guides, and troubleshooting.
3. ***Use Descriptive Filenames:*** Give your documentation files meaningful and descriptive names. Use lowercase letters, hyphens, or underscores to separate words for better readability.
4. ***Include Table of Contents:*** For larger documentation sets, consider adding a table of contents or an index file that provides an overview of all available documentation and serves as an entry point for users.

By following these guidelines, you can effectively document your project on Git, ensuring that important information is well-preserved, easily accessible, and accurately versioned. This helps both current and future developers understand and maintain the project with clarity and efficiency.

### **Further reading**

- [Development tools](./README.md)
- [Project management tool](./Project_Management.md)
- [Docker setup](./Docker_Setup.md)
- [Coding standards](./Coding_Standards.md)
- [Api's](./API's.md)