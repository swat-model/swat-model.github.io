# Set Up Git
## Create Account
Create a free GitHub account at [github.com](https://github.com/), choosing a unique username and providing your email. Opt for the free plan for unlimited public repositories (and private repositories too). Click the top-right profile picture to personalize your profile.

To join the SWAT-Model Research Group on GitHub, reach out to:
**Celray James**: [Profile](https://github.com/celray)
, **Jaclyn**: [Profile](https://github.com/jaclynt)
, **Christoph**: [Profile](https://github.com/chrisschuerz)

For a primer on GitHub, see the ['GitHub Hello World Guide'](https://guides.github.com/activities/hello-world/).

In the next section, we'll discuss using Git for code management. Git allows for changes to local repositories and then pushes to GitHub. An SSH key is essential for a secure connection between your device and GitHub but it is not mandatory.

## Get your code to a repo
You can create your repository on Github web or publish one from any of the methods we will discuss soon.

There are different ways to get your code to Github but in this guide, we briefly mention a few. For more detailed instructions please visit documentation for each of the software mentioned.

### 1. **GitHub Desktop**
This is the easiest method and is recommended for beginners.

Here is how to get code to GitHub using GitHub Desktop:

1. **Setup**
   - Download and install [GitHub Desktop](https://desktop.github.com/).
   - Log in with your GitHub account.
2. **Clone a Repository**
   - Click on `File` > `Clone Repository` from the main menu.
   - Select a repository from the list or enter a repository URL.
3. **Make Changes**
   - Edit files in your preferred text editor.
4. **Commit Changes**
   - Return to GitHub Desktop. It will show changed files.
   - Enter a commit message and description.
   - Click `Commit to master` (or your current branch).
5. **Push Changes**
   - Click the `Push Origin` button at the top.
6. **Syncing**
   - To pull changes from GitHub, click the `Fetch origin` button.

---

### 2. **Visual Studio Code**

This is moderately easy. Here is how to get code to GitHub using Visual Studio Code:

1. **Setup**
   - Install [Visual Studio Code](https://code.visualstudio.com/).
   - Install the [Git extension](https://marketplace.visualstudio.com/items?itemName=vscode.git) if it isn't already.
2. **Clone a Repository**
   - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac).
   - Type `Git: Clone` and paste the repository URL.
3. **Make Changes**
   - Edit files directly within VS Code.
4. **Commit Changes**
   - Click on the source control icon on the sidebar.
   - Enter a commit message.
   - Press the checkmark at the top.
5. **Push Changes**
   - Click on the ellipsis (`...`) > `Push`.
6. **Syncing**
   - Click the sync icon at the bottom left to fetch and integrate changes.

---

### 3. **Command Line**

#### a. Git CLI:

Here is how to get code to GitHub using Git CLI:

1. **Setup**
   - Install [Git](https://git-scm.com/downloads).
2. **Clone a Repository**
   - `git clone [repository-url]`.
3. **Make Changes**
   - Use your preferred text editor to make changes.
4. **Commit Changes**
   - `git add .`
   - `git commit -m "Your commit message here"`.
5. **Push Changes**
   - `git push origin master` (or your current branch).
6. **Syncing**
   - `git pull` to pull changes from GitHub.

#### b. GitHub CLI:

Here is how to get code to GitHub using GitHub CLI:

1. **Setup**
   - Install [GitHub CLI](https://cli.github.com/).
   - Authenticate using `gh auth login`.
2. **Clone a Repository**
   - `gh repo clone [repository-url or owner/repo]`.
3. **Make Changes**
   - Edit files with your preferred text editor.
4. **Commit Changes**
   - `git add .`
   - `git commit -m "Commit message"`.
5. **Push Changes**
   - `git push origin master` (or your current branch).
6. **Open Pull Requests, Issues, etc.**
   - Use various `gh` commands like `gh pr create` or `gh issue create`.

---

Remember, the best method often aligns with your comfort level and the tasks you're trying to accomplish. Starting with GitHub Desktop and progressing to the command line as you become more comfortable can be a great way to gradually build your Git and GitHub skills.
