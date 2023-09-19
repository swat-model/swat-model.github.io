# Collaborating Within the SWAT-Github Organization

---

**Prerequisites** : 

- Make sure you're a member of the GitHub organization.
- Install Git and configure it on your local machine please refer to [This Page](/setup/).

---

## Using GitHub Desktop

---

**Pre-setup**

- Make sure you have [GitHub Desktop](https://desktop.github.com/) installed.
- Log in to GitHub Desktop with your GitHub account that is part of the organization.


**Clone the Repository**

1. Open GitHub Desktop.
2. Go to `File` > `Clone Repository`.
3. Choose the tab for your organization and select the repository to clone.
4. Click `Clone` and choose where you want to save the repository on your local machine.


**Create a New Branch**

1. In GitHub Desktop, ensure you are in the repository you just cloned.
2. Click on the `Current Branch` dropdown in the top bar.
3. Choose `New Branch` and give it a descriptive name.
4. Click `Create Branch`.


**Make Changes**

1. Open the project files in a text editor or Integrated Development Environment (IDE) - Okay, okay fine... Visual Studio Code! If you do not use it, Try today! Don't delay!
2. Make your desired changes and save them.


**Stage and Commit Changes**

1. Return to GitHub Desktop.
2. You will see a list of changed files. You can select the files you want to include in your commit.
3. In the bottom-left corner, write a commit message describing your changes.
4. Click `Commit to [Your Branch Name]`.


**Push to New Branch**

1. Click `Publish branch` or `Push origin` to upload your commits to GitHub.


**Create a Pull Request (PR)**

1. Click on `Create Pull Request` within GitHub Desktop after pushing your changes.
2. This will open a web browser where you can fill in the details of your Pull Request. Click `Create Pull Request` when ready.


**Review and Address Comments**

1. Team members can now review your PR and leave comments on GitHub.
2. To make further changes, return to your text editor or IDE and repeat the process from the "Make Changes" step.
3. Stage, commit, and push these additional changes to update the PR.


**Merging the PR**

1. Once the PR has been approved, someone with the appropriate permissions can merge it on GitHub.
2. After the merge, you'll see an option to delete the remote branch.


**Pull Latest Changes for New Work**

1. Go back to GitHub Desktop.
2. Click on the `Current Branch` dropdown and switch to the `main` or `master` branch.
3. Click `Fetch origin` to pull the latest changes.
4. If there are new updates, click `Pull origin` to update your local branch.

---









## Using VS Code


**Pre-setup**

- Make sure you have [VS Code](https://code.visualstudio.com/) installed.
- Install the [GitHub Pull Requests and Issues](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github) extension from the VS Code marketplace.


**Clone the Repository**

1. Open VS Code.
2. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac) to open the command palette.
3. Type and select `Git: Clone`, then paste the organization's repository URL.
4. Choose a local directory to clone the repository into.


**Create a New Branch**

1. In the lower-left corner of VS Code, click on the branch icon.
2. Select `Create New Branch`.
3. Give your new branch a descriptive name.


**Make Changes**

1. Use VS Code to navigate through the project files.
2. Make your changes using VS Code's text editor.
3. Save your work (`Ctrl+S` or `Cmd+S`).


**Stage and Commit Changes**

1. Click on the source control icon in the sidebar (it looks like a branching fork).
2. You'll see a list of changed files. Stage them by clicking on the `+` next to each file.
3. In the text box at the top, enter a commit message describing your changes.
4. Press the checkmark at the top to commit your changes.


**Push to New Branch**

1. Open the terminal in VS Code (`Ctrl+\`` or `Cmd+\``).
2. Run `git push origin [Your Branch Name]`.


**Create a Pull Request (PR)**

1. Go to the GitHub page of your organization's repository.
2. You'll likely see a prompt to create a new Pull Request; if so, click it.
3. Fill in the PR title and description, then click "Create Pull Request".


**Review and Address Comments**

1. Team members can now review your PR and leave comments on GitHub.
2. Make any necessary changes in VS Code.
3. Stage, commit, and push these changes to the same branch to update the PR.


**Merging the PR**

1. Once the PR is reviewed and approved, someone with the correct permissions can merge it on GitHub.
2. Optionally, you can delete the feature branch from GitHub once it has been merged.


**Pull Latest Changes for New Work**

1. In VS Code, switch back to the `main` branch by clicking on the branch icon in the lower-left corner.
2. Open the terminal and run `git pull origin main`.

---





## Using Command Line
If you feel like being a nerd (we know you do), then this is for you.

**1. Clone the Repository**

- **Why**: To get a local copy of the code on your machine.
- **How**: Open your terminal (Command Prompt, Terminal, Git Bash, etc.) and navigate to the directory where you'd like to place the project.

  ```bash
  git clone https://github.com/swat-model/repository-name.git
  ```


**2. Navigate to the Cloned Directory**

- **Why**: To perform all Git operations inside this directory.
- **How**: Use the `cd` command in your terminal.

  ```bash
  cd repository-name
  ```


**3. Create a New Branch**

- **Why**: To isolate your changes and make collaboration easier.
- **How**: Create and switch to a new branch in your terminal.

  ```bash
  git checkout -b feature-branch-name
  ```


**4. Make Changes**

- **Why**: To implement new features or fix bugs.
- **How**: Open the project in your preferred text editor or IDE and make your changes.


**5. Stage Changes**

- **Why**: To prepare your changes for a commit.
- **How**: Stage all changed files using the `git add` command.

  ```bash
  git add .
  ```
  
  **Note**: Use `git add file-name` to stage individual files.


**6. Commit Changes**

- **Why**: To save your staged changes along with a descriptive message.
- **How**: Commit your changes with a message describing what you've done.

  ```bash
  git commit -m "Implemented feature X"
  ```


**7. Push to the Organization Repository**

- **Why**: To upload your local changes to the remote repository.
- **How**: Push your branch to the remote repository.

  ```bash
  git push origin feature-branch-name
  ```


**8. Create a Pull Request**

- **Why**: To propose that your changes be merged into the main codebase.
- **How**:
  1. Go to the [GitHub page of the swat-model organization's repository](https://github.com/orgs/swat-model/repositories).
  2. Click on "Pull Requests" then "New Pull Request".
  3. Select your branch from the "compare" dropdown.
  4. Add a title and description to your pull request.
  5. Click "Create Pull Request".


**9. Review and Address Feedback**

- **Why**: To ensure code quality and functionality.
- **How**:
  1. Team members review the pull request and provide feedback.
  2. If changes are required, repeat steps 4-7.


**10. Merge the Pull Request**

- **Why**: To include your changes in the project's main codebase.
- **How**: Once your pull request has been reviewed and approved, anyone with merge permissions can merge it.

  ```bash
  Click on "Merge Pull Request" and then "Confirm Merge".
  ```
  

**11. Sync Your Local Main Branch**

- **Why**: To keep your local repository updated.
- **How**: Pull the latest changes from the organization's repository.

  ```bash
  git checkout main
  git pull origin main
  ```

---



## Why Not Commit Directly to the Main Branch?

While it's technically possible to clone a repository and commit directly to the main branch (if you have the necessary permissions), this approach is generally discouraged for the following reasons:

**1. Code Quality and Review**

- Ensuring high code quality, adherence to coding standards, and catching potential bugs or security vulnerabilities. Working on a feature branch and submitting a pull request provides an opportunity for team members to review and comment on your code.

**2. Isolation of Features or Bugs**

- Isolating the development work for specific features or bug fixes. If a feature branch introduces bugs, it won't affect the main codebase, allowing developers time to fix issues before merging.

**3. Concurrent Development**

- Multiple team members can work on different features or bug fixes simultaneously without interference. Each developer works in their own branch, which can later be merged into the main branch after review.

**4. Rollback and History Clarity**

- Easier to roll back features or changes when they are isolated in their own branches. Git history will clearly show each feature as a merge commit from a branch, making it easier to identify and revert, if necessary.

**5. Access Control and Permissions**

- Control over who can commit directly to the main branch, which should represent the stable version of the project. Setting branch protection rules allows control over who can push to the main or master branches and requires certain checks to pass before merging.

**6. Prevent Unstable Code**

- Direct commits to the main branch can result in an unstable or broken codebase, affecting all team members. Feature branches must pass continuous integration tests and get approved through code review before merging into the main branch.

**7. Documentation and Understanding**

- Pull requests provide a forum for discussing the proposed changes, adding to the project's documentation and understanding. The discussion on a pull request can be referred to in the future for context, serving as valuable project documentation.

For these reasons, the best practice is to clone the repository, create a new branch for your feature or fix, commit your changes to that branch, and then open a pull request for review. After approval, the changes can then be merged into the main or master branch.
