
# KCS GitHub Flow for New Developers

This guide will help you get started with the GitHub flow of KCS. Follow the steps below to get started.

---

## 1. Cloning the Repository

All work related to KCS should be cloned into a dedicated `KCS` directory on your local machine:

```sh
git clone <repository_url>
```

Navigate into the cloned repository:

```sh
cd KCS/<repository_name>
```

Ensure that you have the latest version of the repository:

```sh
git pull origin main
```

---

## 2. Creating a New Branch

The `main` branch is our production branch and should never be committed to directly. Instead, follow these steps:

1. Create a new branch for your feature or bug fix:

   ```sh
   git checkout -b feature/your-feature-name
   ```

2. Follow the branch naming conventions:
   - `feature/your-feature-name` for new features
   - `bugfix/your-bug-description` for bug fixes
   - `hotfix/critical-fix-description` for urgent fixes

3. Regularly pull the latest changes from `main` to keep your branch up to date:

   ```sh
   git pull origin main
   ```

---

## 3. Making Code Changes

1. Make your changes in the appropriate files.
2. Stage your changes:

   ```sh
   git add .
   ```

3. Commit with a meaningful message:

   ```sh
   git commit -m "[Feature] Add user authentication"
   ```

4. Push your branch to GitHub:

   ```sh
   git push origin feature/your-feature-name
   ```

---

## 4. Creating a Pull Request (PR)

1. Go to the repository on GitHub.
2. Navigate to the "Pull Requests" tab.
3. Click "New Pull Request" and select your branch.
4. Follow the PR naming conventions and rules:
   - `[Feature] Add feature description`
   - `[Bugfix] Fix issue description`
   - `[Hotfix] Quick fix description`
5. Add a detailed description of your changes.
6. Assign reviewers and request a review.

Once approved, your code can be merged into `main`.

---

## 5. Merging and Cleaning Up

1. Ensure your branch is up to date with `main` before merging.
2. Merge the PR via GitHub.
3. Delete the branch locally and remotely:

   ```sh
   git branch -d feature/your-feature-name
   git push origin --delete feature/your-feature-name
   ```

---

## 6. Best Practices

- **Always pull the latest changes** before starting work.
- **Use descriptive commit messages** for easy tracking.
- **Break down large features** into smaller branches for better management.
- **Follow code review guidelines** before merging PRs.
- **Regularly sync your branch** with `main` to avoid merge conflicts.
- **Write tests** where applicable to ensure code stability.

Following these steps will ensure a smooth development workflow and effective collaboration within the team. 🚀
