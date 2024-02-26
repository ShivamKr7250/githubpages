# GitHub Workshop README

Welcome to our GitHub Workshop! This README will serve as your guide to understanding the basics of Git and GitHub, including how to install Git on your machine, and an overview of important Git commands you'll be using throughout this workshop. Let's dive in!

## What are Git and GitHub?

**Git** is a distributed version control system that allows you to track changes in your files and coordinate work on those files among multiple people. It's a fundamental tool for developers, allowing for efficient collaboration and version control of projects.

**GitHub** is a cloud-based hosting service that lets you manage Git repositories. It provides a web-based graphical interface and includes features such as bug tracking, feature requests, task management, and wikis for every project. GitHub makes collaboration on code projects easier, offering tools for reviewing code, managing projects, and hosting documentation.

## Installing Git

### Windows

1. Download the latest Git for Windows installer from the [Git website](https://git-scm.com/download/win).
2. Run the installer and follow the steps provided by the setup wizard. Leave all the default settings unless you have a specific need to change them.
3. To check if Git was installed successfully, open the Command Prompt or Git Bash and type `git --version`.

### macOS

1. The easiest way to install Git on a Mac is through the stand-alone installer:
   - Download the latest macOS Git installer from the [Git website](https://git-scm.com/download/mac).
   - Follow the prompts to install Git.
2. Alternatively, you can use Homebrew by running `brew install git` in the terminal.
3. Verify the installation by opening the Terminal and typing `git --version`.

### Linux

1. Open a terminal window.
2. Update your package list with `sudo apt-get update` (Debian/Ubuntu) or `sudo yum update` (Fedora).
3. Install Git using `sudo apt-get install git` (Debian/Ubuntu) or `sudo yum install git` (Fedora).
4. Confirm the installation by typing `git --version`.

## Configuring Git

Before starting to use Git, you'll need to configure your user name and email address. Run the following commands, replacing the name and email with your own:

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

## Important Git Commands

- **`git init`**: Initialize a new Git repository in your current directory.
- **`git clone [URL]`**: Clone (copy) a repository from GitHub (or another location) to your local machine.
- **`git add [file]`**: Add a file(s) to the staging area, marking it for inclusion in the next commit.
- **`git commit -m "[commit message]"`**: Commit your staged changes to the repository along with a descriptive message.
- **`git push`**: Push your local commits to the remote repository on GitHub.
- **`git pull`**: Update your local repository with the newest commits from the remote repository.
- **`git branch`**: List, create, or delete branches.
- **`git checkout [branch-name]`**: Switch to another branch and check it out into your working directory.
- **`git merge [branch]`**: Merge the specified branch’s history into the current branch.

## Additional Resources

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Learning Lab](https://lab.github.com/)
- [Pro Git Book](https://git-scm.com/book/en/v2)


# Working with Git and GitHub: Cloning, Forking, and Contributing

Welcome! This README is designed to guide you through the processes of cloning a repository, forking a repository, making changes, and contributing those changes back to the original project via a pull request on GitHub.

## Cloning a Repository

**Cloning** a repository means making a copy of the repository on your local machine. This allows you to work on the project files locally.

### How to Clone a Repository

1. Navigate to the main page of the repository on GitHub.
2. Above the list of files, click the **Code** button.
3. To clone the repository using HTTPS, under "Clone with HTTPS", click the clipboard icon. To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click the clipboard icon.
4. Open your terminal.
5. Change the current working directory to the location where you want the cloned directory.
6. Type `git clone`, and then paste the URL you copied earlier.
   
   ```
   git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
   ```

7. Press **Enter** to create your local clone.

## Forking a Repository

**Forking** a repository allows you to freely experiment with changes without affecting the original project. It creates a copy of the repository in your GitHub account.

### How to Fork a Repository

1. Navigate to the GitHub page of the repository you want to fork.
2. In the top-right corner of the page, click the **Fork** button.
3. You will be redirected to your forked version of the repository.

## Making Changes and Pushing to Your Fork

After forking a repository, you can make changes to your fork and push them to GitHub.

### Making Changes

1. Navigate to the cloned directory if you haven’t already:

   ```
   cd YOUR-REPOSITORY
   ```

2. Create a new branch to make your changes on:

   ```
   git checkout -b your-new-branch-name
   ```

3. Make your changes in the repository files with your preferred text editor or IDE.

4. After making changes, stage them for commit:

   ```
   git add .
   ```

5. Commit the changes with a meaningful message:

   ```
   git commit -m "Add your commit message"
   ```

### Pushing Changes

1. Push your branch and changes to your fork on GitHub:

   ```
   git push origin your-new-branch-name
   ```

## Creating a Pull Request

After pushing your changes, you can submit a pull request to the original repository to propose your changes.

### How to Create a Pull Request

1. Navigate to your fork on GitHub.
2. Click the **Pull requests** tab and then click **New pull request**.
3. In the "base repository" dropdown menu, select the original repository you’d like to contribute to. In the "base" dropdown menu, select the branch of the original repository you’d like to contribute to. In the "head repository" dropdown menu, select your fork, and in the "compare" dropdown menu, select your branch.
4. Review the changes and ensure they are correct.
5. Click **Create pull request**.
6. Add a title and description to your pull request explaining your changes.
7. Click **Create pull request** again.

Congratulations! You've now learned how to clone a repository, fork a repository, make changes, push them back to your repo, and create a pull request to contribute to the original project.
