# **Level 2: Basic Operations** ⚙️

Now that you're familiar with the basics, let's dive deeper into the essential Git and GitHub operations that you’ll frequently use while working with repositories!

### **Topics Covered:**
1. **Cloning a Repository** 🖥️
2. **Making Commits and Pushing Changes** 🔄
3. **Creating and Merging Branches** 🌿
4. **Handling Merge Conflicts** ⚔️

---

## **1. Cloning a Repository** 🖥️

**Cloning** a repository means creating a local copy of a remote repository on your own computer. This allows you to work on the project offline and push changes back to GitHub when you're ready.

Here’s how you can clone a repository:

1. **Navigate to the repository page** on GitHub. 🌐
2. Click the green **Code** button. 🟩
3. Copy the **URL** under "Clone with HTTPS." 🔗
4. Open your terminal (or Git Bash) and type the following command:

    ```bash
    git clone https://github.com/username/repository-name.git
    ```

5. Press **Enter**. This will create a local copy of the repository on your machine, and you can start working on it. 💻

---

## **2. Making Commits and Pushing Changes** 🔄

Once you've made changes to your files, you need to **commit** them. A commit is like saving your work, and you should always write meaningful commit messages.

Here’s how to commit and push changes:

1. **Track changes** to files by running:

    ```bash
    git add <file-name>
    ```

    To add all files at once, use:

    ```bash
    git add .
    ```

2. **Commit** your changes with a descriptive message:

    ```bash
    git commit -m "Your commit message"
    ```

3. **Push** the changes to the remote repository on GitHub:

    ```bash
    git push origin main
    ```

    This sends your local commits to the remote repository, updating it with your changes. 🚀

---

## **3. Creating and Merging Branches** 🌿

Git allows you to work on different parts of a project without affecting the main codebase. **Branches** are used for this purpose. You can create a branch for new features or fixes, and once you're done, you can merge it back into the main branch.

### **Creating a Branch:** 

1. To create a new branch, run:

    ```bash
    git checkout -b <branch-name>
    ```

2. After making changes, **commit** them as usual and push the branch to GitHub:

    ```bash
    git push origin <branch-name>
    ```

### **Merging a Branch:** 

Once you've finished working on your branch, you can merge it back into the main branch.

1. First, **switch to the main branch**:

    ```bash
    git checkout main
    ```

2. Then, **merge the branch**:

    ```bash
    git merge <branch-name>
    ```

3. Finally, push the merged changes to GitHub:

    ```bash
    git push origin main
    ```

---

## **4. Handling Merge Conflicts** ⚔️

Sometimes, when you try to merge branches, **merge conflicts** can occur. This happens when the same part of a file has been modified in both branches. Git will ask you to resolve these conflicts manually.

Here’s how to handle merge conflicts:

1. **Identify the conflict** by running:

    ```bash
    git status
    ```

    Git will highlight the files with conflicts. 🚨

2. Open the conflicted files. You'll see sections like:

    ```plaintext
    <<<<<<< HEAD
    Your changes
    =======
    Changes from the other branch
    >>>>>>> branch-name
    ```

3. Manually edit the file to combine the changes or choose one version over the other. After resolving the conflict, **save** the file. 📝

4. Mark the conflict as resolved by adding the file:

    ```bash
    git add <file-name>
    ```

5. Commit the resolution:

    ```bash
    git commit -m "Resolved merge conflict"
    ```

6. Finally, push the changes:

    ```bash
    git push origin main
    ```

---

## **Conclusion** 🎉

In this level, you learned how to perform basic Git operations like cloning a repository, making commits and pushing changes, creating and merging branches, and handling merge conflicts. These are some of the core tasks you'll perform regularly when working with GitHub.

👉 **Next:** Move on to [Level 3: Collaboration](../Level-3_Collaboration/README.md) to learn how to collaborate effectively with others on GitHub. 🤝
