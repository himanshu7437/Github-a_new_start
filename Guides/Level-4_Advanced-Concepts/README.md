# **Level 4: Advanced Concepts**

Master the advanced features of GitHub and elevate your workflow to the next level. In this level, you'll learn about powerful tools and techniques that streamline development and enhance your productivity.

### **Topics Covered:**
1. **Git Rebase and Squash**
2. **GitHub Actions for Automation**
3. **Hosting with GitHub Pages**
4. **Using .gitignore and Git LFS**

---

## **1. Git Rebase and Squash**

**Git Rebase** and **Git Squash** are advanced techniques used to modify commit history in Git. These tools are useful for cleaning up commit history before merging branches and keeping your Git history linear and readable.

### **Git Rebase:**

Rebasing is the process of moving or combining a sequence of commits to a new base commit. Instead of merging, rebase re-applies changes from one branch onto another branch.

1. To rebase your current branch onto the latest commit from another branch (e.g., main):

    ```bash
    git checkout <your-branch>
    git rebase main
    ```

2. If conflicts occur, resolve them manually, then use:

    ```bash
    git rebase --continue
    ```

### **Git Squash:**

Squashing combines multiple commits into one, making the commit history more concise. This is typically used for cleaning up commits before merging a feature branch.

1. Start an interactive rebase:

    ```bash
    git rebase -i <commit-id>
    ```

2. Mark the commits you want to squash with `s` (for squash) or `f` (for fixup).
3. After squashing, push the changes:

    ```bash
    git push origin <your-branch> --force
    ```

---

## **2. GitHub Actions for Automation**

**GitHub Actions** is a feature that allows you to automate workflows, such as building, testing, and deploying code directly from your GitHub repository. It’s based on YAML configuration files that define your workflows.

### **Setting Up a Basic GitHub Action:**

1. Go to the **Actions** tab of your GitHub repository.
2. Click **New Workflow** and choose a template or create a custom YAML file.
3. Define the steps, such as running tests, deploying code, or building your project. Here’s an example of a simple workflow for running tests:

    ```yaml
    name: Run Tests

    on:
      push:
        branches:
          - main

    jobs:
      test:
        runs-on: ubuntu-latest
        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Set up Node.js
            uses: actions/setup-node@v2
            with:
              node-version: '14'
          - name: Install dependencies
            run: npm install
          - name: Run tests
            run: npm test
    ```

This YAML configuration runs tests every time changes are pushed to the `main` branch.

---

## **3. Hosting with GitHub Pages**

**GitHub Pages** allows you to host static websites directly from a GitHub repository. It’s an easy way to showcase projects, portfolios, or documentation.

### **Steps to Host a Website:**

1. Create a new branch named `gh-pages` (or use the `main` branch).
2. Add your static website files (HTML, CSS, JS) to the repository.
3. Go to your repository settings.
4. Under the **GitHub Pages** section, select the branch (usually `main` or `gh-pages`) to deploy from.
5. Your website will be live at `https://username.github.io/repository-name`.

---

## **4. Using .gitignore and Git LFS**

### **.gitignore:**

A `.gitignore` file tells Git which files or directories to ignore when committing changes. This is useful for excluding temporary files, build files, and sensitive data.

1. Create a `.gitignore` file in the root of your repository.
2. Add the patterns for the files you want to exclude. For example:

    ```
    # Ignore Node.js dependencies
    node_modules/

    # Ignore log files
    *.log
    ```

3. Save the `.gitignore` file and commit it to your repository. Git will ignore the files specified in this file.

### **Git LFS (Large File Storage):**

Git LFS is an extension for Git to manage large files, such as videos, images, or datasets, that would otherwise slow down the repository.

1. Install Git LFS:

    ```bash
    git lfs install
    ```

2. Track a specific file type with LFS (e.g., images):

    ```bash
    git lfs track "*.png"
    ```

3. Commit the `.gitattributes` file that Git LFS creates to your repository.
4. Git LFS will automatically handle large files for you.

---

## **Conclusion**

Congratulations! You’ve mastered advanced GitHub features such as Git rebase, GitHub Actions for automation, hosting with GitHub Pages, and using `.gitignore` and Git LFS for handling large files. These powerful tools help improve your development workflow and allow you to collaborate more efficiently.

🎯 **Congratulations!** You've completed the guide. Explore [Challenges](../../challenges/) next to put your knowledge into practice!
