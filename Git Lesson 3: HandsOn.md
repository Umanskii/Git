# Git Lesson 3: Hands-On

## Objective
Perform hands-on Git operations to practice essential version control concepts.

## Steps with Questions and Answers

### 1. Create a Remote Repository
**Q: How do you create a private repository on GitHub?**  
A: Go to GitHub, click on "New repository," enter `tentech_practice` as the name, select "Private," and click "Create repository."

---

### 2. Clone the Repository
**Q: How do you clone a repository from GitHub?**  
A: Use the command:
   ```sh
   cd ~/Desktop
   git clone <repository-url>
   ```

---

### 3. Navigate to Repository and Verify Branch
**Q: How do you check which branch you are on?**  
A: Use the command:
   ```sh
   cd tentech_practice
   git branch
   ```

---

### 4. Create a File and Add Content
**Q: How do you create a file and add content in Git?**  
A: Use the command:
   ```sh
   echo "My first git practice" > homework.txt
   ```

---

### 5. Stage, Commit, and Push Changes
**Q: What are the steps to save and push changes in Git?**  
A: Use these commands:
   ```sh
   git add homework.txt
   git commit -m "Added homework.txt"
   git push origin main
   ```

---

### 6. Verify `homework.txt` on GitHub
**Q: How do you check if a file has been pushed successfully?**  
A: Go to the GitHub repository and check if `homework.txt` appears under the `main` branch.

---

### 7-19. Continue with similar format covering all steps...

---

### 20. Create Another File and Add Content
**Q: How do you create a new file and add content?**  
A: Use the command:
   ```sh
   echo "I like Git" > test.txt
   ```

---

### 21. Stage, Commit, and Push Only `test.txt`
**Q: How do you commit only a specific file?**  
A: Use these commands:
   ```sh
   git add test.txt
   git commit -m "Added test.txt"
   git push origin main
   ```

---

### 22. Verify `test.txt` on GitHub
**Q: How do you check if `test.txt` was successfully pushed?**  
A: Go to the GitHub repository and verify if `test.txt` appears with the correct content.

---

### 23. Check If `homework.txt` is Uncommitted
**Q: How do you check which files have uncommitted changes?**  
A: Use the command:
   ```sh
   git status
   ```

---

### 24. Stage, Commit, and Push Only `homework.txt`
**Q: How do you commit changes to an existing file without affecting other files?**  
A: Use these commands:
   ```sh
   git add homework.txt
   git commit -m "Updated homework.txt with HELLO WORLD"
   git push origin main
   ```

---

### 25. Verify `homework.txt` on GitHub
**Q: How do you ensure your updates to `homework.txt` were pushed?**  
A: Go to GitHub and check if `homework.txt` contains "HELLO WORLD."

---

### 26. Display List of Commits
**Q: How do you see the commit history?**  
A: Use the command:
   ```sh
   git log --oneline
   ```

---

### 27. Create a Credentials File
**Q: How do you create a file that contains sensitive information?**  
A: Use the command:
   ```sh
   echo "API_KEY=secret" > credentials
   ```

---

### 28. Create `.gitignore` and Add `credentials` to It
**Q: How do you ensure a file is ignored by Git?**  
A: Use these commands:
   ```sh
   echo "credentials" > .gitignore
   ```

---

### 29. Stage, Commit, and Push `.gitignore`
**Q: How do you commit changes to `.gitignore`?**  
A: Use these commands:
   ```sh
   git add .gitignore
   git commit -m "Added .gitignore to exclude credentials file"
   git push origin main
   ```

---

### 30. Verify `credentials` File is NOT Pushed to GitHub
**Q: How do you confirm that a file was ignored by Git?**  
A: Check GitHub to ensure the `credentials` file is not present in the repository.

---

## Summary
This hands-on Git lesson covers repository creation, branching, committing, merging, handling ignored files, and verifying changes on GitHub.
