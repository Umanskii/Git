To complete this Git-based task, you can follow these step-by-step instructions. I will break down each step clearly to help you get through it.

### 1. Create a remote private repo on your GitHub called `tentech_practice`
- Go to your GitHub account, click on the **+** in the top right, and select **New repository**.
- Name the repository `tentech_practice` and set it to **private**.
- Click **Create repository**.

### 2. Clone the repository to your local machine
- Open the terminal and navigate to the `~/Desktop` directory:
  ```bash
  cd ~/Desktop
  ```
- Clone your repository:
  ```bash
  git clone https://github.com/your-username/tentech_practice.git
  ```

### 3. Navigate to your repo directory and verify if you are in the `main` branch
- Change to the repo directory:
  ```bash
  cd tentech_practice
  ```
- Verify if you are in the `main` branch:
  ```bash
  git branch
  ```
  It should show `* main` (indicating that you are currently on the `main` branch).

### 4. Create a `homework.txt` file and add content to it
- Run the following command:
  ```bash
  echo "My first git practice" > homework.txt
  ```

### 5. Commit changes to GitHub
- Stage the changes:
  ```bash
  git add homework.txt
  ```
- Commit the changes:
  ```bash
  git commit -m "Add homework.txt with first line"
  ```
- Push the changes to GitHub:
  ```bash
  git push origin main
  ```

### 6. Verify the file on GitHub
- Go to the `tentech_practice` repo on GitHub and check if `homework.txt` appears with "My first git practice" inside.

### 7. Create a new branch called `practice`
- Run the following command to create the new branch:
  ```bash
  git checkout -b practice
  ```

### 8. Verify if you are in the `practice` branch
- Run:
  ```bash
  git branch
  ```
  It should show `* practice`.

### 9. Add a second line to the `homework.txt` file
- Run the command:
  ```bash
  echo "Tentech is the best DevOps school" >> homework.txt
  ```

### 10. Commit changes to GitHub
- Stage the changes:
  ```bash
  git add homework.txt
  ```
- Commit the changes:
  ```bash
  git commit -m "Add second line to homework.txt"
  ```
- Push the `practice` branch to GitHub:
  ```bash
  git push origin practice
  ```

### 11. Verify the file on GitHub (on the `practice` branch)
- Go to GitHub, switch to the `practice` branch, and verify if `homework.txt` contains the second line "Tentech is the best DevOps school".

### 12. Create a New Pull Request
- On GitHub, create a **Pull Request** from the `practice` branch to `main`.

### 13. Verify changes in the "Files changed" tab
- Check the **Files changed** tab to verify the changes.

### 14. Approve and merge the Pull Request, and delete the `practice` branch
- Approve and merge the Pull Request.
- After merging, you can delete the `practice` branch from GitHub.

### 15. Verify the changes on the `main` branch
- Switch to the `main` branch and check if the second line is merged:
  ```bash
  git checkout main
  git pull origin main
  cat homework.txt
  ```

### 16. Delete the `practice` branch locally
- Since the branch no longer exists on GitHub, run:
  ```bash
  git branch -d practice
  ```

### 17. Verify there is only the `main` branch
- Run:
  ```bash
  git branch
  ```
  It should only show `main`.

### 18. Check the `homework.txt` file
- Make sure the `homework.txt` file has 2 lines. If not, run:
  ```bash
  git pull origin main
  ```

### 19. Add a 3rd line to the `homework.txt` file
- Run:
  ```bash
  echo "HELLO WORLD" >> homework.txt
  ```

### 20. Create a second file: `test.txt`
- Run:
  ```bash
  echo "I like Git" > test.txt
  ```

### 21. Commit `test.txt` file to GitHub
- Stage the changes:
  ```bash
  git add test.txt
  ```
- Commit the changes:
  ```bash
  git commit -m "Add test.txt"
  ```
- Push the changes:
  ```bash
  git push origin main
  ```

### 22. Verify the `test.txt` file on GitHub
- Go to GitHub and check if `test.txt` is there with the content "I like Git".

### 23. Check if `homework.txt` changes are committed
- Run:
  ```bash
  git status
  ```
  It should indicate if any changes in `homework.txt` are not committed yet.

### 24. Commit `homework.txt` changes to GitHub
- If necessary, stage and commit any changes in `homework.txt`:
  ```bash
  git add homework.txt
  git commit -m "Update homework.txt with HELLO WORLD"
  git push origin main
  ```

### 25. Verify `homework.txt` on GitHub
- Ensure the file has "HELLO WORLD" inside.

### 26. Display a list of commits
- Run:
  ```bash
  git log
  ```

### 27. Create a credentials file
- Create a file called `credentials.txt` with some sensitive information inside.

### 28. Set up `.gitignore` to ignore the `credentials.txt` file
- Create a `.gitignore` file if not already created and add the `credentials.txt` file to it:
  ```
  credentials.txt
  ```

### 29. Stage, commit, and push your changes to the remote repo
- Stage the changes:
  ```bash
  git add .gitignore credentials.txt
  ```
- Commit the changes:
  ```bash
  git commit -m "Add .gitignore to ignore credentials.txt"
  ```
- Push to GitHub:
  ```bash
  git push origin main
  ```

### 30. Verify if the `credentials.txt` file is not pushed to the remote repo
- Verify that `credentials.txt` is not in the GitHub repository.

These steps should guide you through the task. Let me know if you need further clarification on any of the steps!
