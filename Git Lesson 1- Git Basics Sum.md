# Git Basics - Lesson 1

## **1. Version Control & Git Basics**
### **What is Git?**
- A distributed version control system for tracking code changes and collaboration.
- Works locally and allows easy rollback to previous versions.

### **What is GitHub?**
- A cloud-based platform that hosts Git repositories and adds collaboration features like pull requests and issue tracking.
- Acts like Google Drive for Git repositories.

## **2. Git Architecture: Three Stages**
1. **Working Directory:** Where changes are made.
2. **Staging Area:** Selected changes prepared for commit (`git add`).
3. **Local Repository:** Committed changes are saved locally (`git commit`).
4. **Remote Repository:** Shared repository on GitHub (`git push`).

## **3. Key Git Commands**
### **Initialize a Git repository**  
```sh
git init
```
### **Check status of changes**  
```sh
git status
```
### **Add files to staging area**  
```sh
git add <file>
```
### **Commit changes**  
```sh
git commit -m "Message"
```
### **Push changes to remote repository**  
```sh
git push origin <branch>
```
### **Create and switch branches**  
```sh
git branch <branch-name>
git checkout <branch-name>
```
### **Merge branches**  
```sh
git merge <branch-name>
```

## **4. Git Workflow & Collaboration**
- **Branching:** Developers work on separate branches to avoid conflicts.
- **Merging:** Combines work from different branches.
- **Pull Requests:** Used on GitHub to propose and review changes.

## **5. Git Best Practices**
- **Commit Often:** Save progress regularly.
- **Use Descriptive Messages:** Clear commit messages help track changes.
- **Group Related Changes:** Separate commits for different updates.
- **.gitignore:** Exclude unnecessary files from version control.

---
🚀 This lesson provides a solid foundation in Git version control, helping developers track changes, collaborate, and manage code efficiently.
