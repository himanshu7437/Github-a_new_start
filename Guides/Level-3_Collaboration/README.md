# **Level 3: Collaboration** 🤝

Collaboration is key to working with others on GitHub! In this level, you will learn how to effectively collaborate on projects using various GitHub features that enable teamwork and communication.

### **Topics Covered:**
1. **Forking Repositories** 🍴
2. **Creating and Reviewing Pull Requests** 🔄
3. **Issue Tracking and Labels** 📝
4. **Collaborating with Teams** 👥

---

## **1. Forking Repositories** 🍴

**Forking** is a process where you create a personal copy of someone else's repository. It allows you to freely experiment with changes without affecting the original project. Forking is a fundamental part of collaborating on open-source projects.

Here’s how to fork a repository:

1. **Navigate to the repository** you want to fork on GitHub.
2. In the top-right corner, click the **Fork** button.
3. GitHub will create a copy of the repository under your GitHub account.
4. Now, you can clone this forked repository to your local machine and make changes to it.

To keep your fork up to date with the original repository:

1. Add the original repository as a **remote**:

    ```bash
    git remote add upstream https://github.com/owner/repository.git
    ```

2. Fetch the latest changes:

    ```bash
    git fetch upstream
    ```

3. Merge the updates into your local repository:

    ```bash
    git merge upstream/main
    ```

---

## **2. Creating and Reviewing Pull Requests** 🔄

Once you’ve made changes to your forked repository or branch, you can submit a **pull request** (PR) to suggest your changes to the original repository.

### **Creating a Pull Request:**

1. Go to the **Pull Requests** tab in the repository on GitHub.
2. Click **New Pull Request**.
3. Select the branch from your fork that contains the changes and compare it with the base repository's main branch.
4. Write a clear title and description for the PR explaining what changes you’ve made.
5. Click **Create Pull Request**.

### **Reviewing a Pull Request:**

1. In the **Pull Requests** tab, select the PR you want to review.
2. GitHub shows the differences between the branches.
3. You can leave comments on specific lines of code or give general feedback.
4. Once the review is done, you can either approve the changes or request further modifications.
5. If everything looks good, you can merge the PR.

---

## **3. Issue Tracking and Labels** 📝

GitHub provides an issue tracking system that allows you to create and track bugs, tasks, and feature requests. Issues can be tagged with labels to categorize and prioritize them.

### **Creating an Issue:**

1. Navigate to the **Issues** tab in the repository.
2. Click **New Issue**.
3. Fill in the title and description of the issue.
4. Submit the issue.

### **Using Labels:**

Labels help organize and prioritize issues. Common labels include "bug," "enhancement," and "help wanted." You can add labels to an issue when creating it, or you can edit an existing issue to add labels.

### **Assigning Issues:**

You can assign issues to team members so they know who is responsible for addressing the issue. This helps in managing tasks and tracking progress.

---

## **4. Collaborating with Teams** 👥

GitHub also provides features for working within teams, particularly useful for organizations or larger projects.

### **Creating a Team:**

1. In your organization, go to the **Teams** tab.
2. Click **New Team** and give it a name and description.
3. Add members to the team.

### **Assigning Permissions:**

GitHub allows you to set specific **permissions** for teams. You can choose from:
- **Read:** Can view the repository but cannot make changes.
- **Write:** Can push changes to the repository.
- **Admin:** Has full control over the repository, including managing teams and settings.

### **Collaborative Features:**

- **Discussions:** Teams can engage in discussions and ask questions using GitHub Discussions.
- **Code Review:** Team members can perform code reviews by reviewing pull requests and providing feedback.

---

## **Conclusion** ✅

In this level, you learned how to collaborate effectively on GitHub by forking repositories, creating and reviewing pull requests, using issue tracking and labels, and collaborating with teams. These skills are essential for working with others on open-source projects or in a team setting.

👉 **Next:** Move on to [Level 4: Advanced Concepts](../Level-4_Advanced-Concepts/README.md) to explore more advanced Git and GitHub features.
