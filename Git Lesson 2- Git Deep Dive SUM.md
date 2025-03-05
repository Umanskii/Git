# Git Deep Dive - Lesson 2

## **1. Git Branching**
- Branches enable isolated development without affecting the main codebase.
- The default branch is usually **master** (or **main**).
- Create a new branch:  
  ```sh
  git branch <branch-name>
  ```
- Switch to an existing branch:  
  ```sh
  git checkout <branch-name>
  ```
- Alternative (`Git 2.23+`):  
  ```sh
  git switch <branch-name>
  ```

## **2. Git Merging**
- Merging integrates changes from one branch into another.
- **Fast-forward merge** occurs when there’s a direct path between branches.
- **Three-way merge** happens when branches have diverged, requiring Git to create a merge commit.
- Merge conflicts occur when two branches modify the same line of code.

## **3. Merge Conflicts & Resolution**
- Conflict markers:  
  ```sh
  <<<<<<< HEAD
  =======
  >>>>>>> branch-name
  ```
- Identify conflicts:
  ```sh
  git status
  ```
- Resolve conflicts manually, then mark them as resolved:
  ```sh
  git add <conflicted-file>
  ```
- Abort a merge:
  ```sh
  git merge --abort
  ```

## **4. Git Stash**
- Temporarily stores uncommitted changes:
  ```sh
  git stash
  ```
- Apply stashed changes and remove them:
  ```sh
  git stash pop
  ```
- Apply stashed changes without removing them:
  ```sh
  git stash apply
  ```

## **5. Reverting Changes**
- Revert a specific commit:
  ```sh
  git revert <commit-hash>
  ```
- Reset moves the branch pointer:
  - **Soft reset** (keeps changes staged):
    ```sh
    git reset --soft HEAD~1
    ```
  - **Hard reset** (removes all changes):
    ```sh
    git reset --hard HEAD~1
    ```
- Use `git revert` for shared/public branches to maintain history integrity.

## **6. Git Rebase (Optional)**
- Alternative to merging that creates a linear history.
- Rebase the current branch onto `main`:
  ```sh
  git rebase main
  ```
- Interactive rebase (modify commit history):
  ```sh
  git rebase -i main
  ```
- **Golden Rule**: Never rebase a public branch, as it rewrites history.

---
🚀 This guide provides foundational knowledge for effective Git branching, merging, conflict resolution, and history management.
