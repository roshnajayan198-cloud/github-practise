# Guide to Making Your First Open Source Contribution (Git & GitHub PR Workflow)

Welcome! This guide walks you through the step-by-step process of contributing to an open-source project or repository. Following these steps ensures your work remains clean, organized, and easy for project maintainers to review.

---

## 🚀 Part 1: Getting the Code Onto Your Computer

Before you change any code, you need to create a personal copy of the project to safely experiment with.

### Step 1: Fork the Repository
1. Navigate to the main GitHub page of the project you want to contribute to.
2. In the top-right corner, click the **Fork** button.
3. This creates an exact copy of their repository inside your personal GitHub account.

### Step 2: Clone Your Forked Copy
1. Go to **your** forked version of the project on GitHub.com (the URL will look like `https://github.com/YOUR-USERNAME/PROJECT-NAME`).
2. Click the green **<> Code** button and copy the HTTPS URL provided.
3. Open your Terminal or Command Prompt and run the following command to download it to your computer:
```bash
   git clone [https://github.com/YOUR-USERNAME/PROJECT-NAME.git](https://github.com/YOUR-USERNAME/PROJECT-NAME.git)

Step 3: Navigate into the Project Folder
Move your terminal's focus into the newly created folder:

Bash
   cd PROJECT-NAME
🛠️ Part 2: Working Safely with Branches
Never make changes directly to the main or master branch. Always create a dedicated "feature branch" for your task so your changes stay isolated.

Step 4: Create and Switch to a New Branch
Think of a short, descriptive name for your task (e.g., extract-flood-engine or fix-loading-bug).

Run the following command:

Bash
   git checkout -b your-feature-branch-name
(The -b flag tells Git to create a brand-new branch and immediately switch you into it).

Step 5: Make Your Code Changes
Open the project folder in your preferred code editor (e.g., VS Code).

Complete your task (e.g., create new files, move JavaScript logic, update HTML scripts).

Test your changes locally to ensure the website or application still runs perfectly without any unexpected bugs.

📤 Part 3: Saving and Uploading Your Work
Once your code edits are complete and tested, you need to save your progress with Git and upload it back up to GitHub.

Step 6: Stage Your Modified Files
Check which files you altered by running git status.

Stage all your changes to prepare them for a save:

Bash
   git add .
Step 7: Commit Your Changes
Save your changes with a clear, concise message describing exactly what you did:

Bash
   git commit -m "Extract traffic jam risk logic into separate js file"
Step 8: Push Your Branch to GitHub
Upload your local feature branch up to your forked copy on GitHub:

Bash
   git push origin your-feature-branch-name
🤝 Part 4: Creating the Pull Request (PR)
Now that your modified code is sitting on GitHub, you are ready to officially propose your changes to the project maintainers.

Step 9: Open the Pull Request on GitHub
Open your web browser and go back to your forked repository page on GitHub.com.

A yellow alert bar should appear at the top showing your recently pushed branch. Click the green Compare & pull request button next to it.

If you do not see the banner, click on the Branches tab or dropdown, switch to your feature branch, and hit New pull request.

Step 10: Complete the PR Title and Description
Give your PR a clear title (e.g., Extract flood risk into js/flood-engine.js).

In the description box, write a friendly summary of what you did.

Pro-Tip: Include a magic linking keyword to automatically link and close your target issue when your PR gets approved. For example:

Markdown
   Closes #8

   ### Description
   Moved the requested flood risk variables and helper functions out of the inline script block in `index.html` and placed them into a clean, modular `js/flood-engine.js` file. Added the new script reference to `index.html`. Verified that the UI works identically!
Click the green Create pull request button.
