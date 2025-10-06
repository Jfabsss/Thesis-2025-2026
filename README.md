# Git Basics

Clone the repository and get set up:

```
git clone git@github.com:Jfabsss/Thesis-2025-2026.git
git fetch
git checkout testing
git pull

```

### Workflow for Making Changes
1. Create a new branch from the testing branch
Example:

```
git checkout -b feat/registration-page testing

```

2. Fetch the latest branches

```

git fetch

```
3. Make your changes
Add your feature or fix your bug here.

4. Stage files (avoid git add .)
Be specific when staging:

```
git add file1.tsx file2.tsx .gitignore
```

5. Commit your changes
Use a clear commit message format:

For fixes:
```
git commit -m "fix: corrected button alignment"
```

For features:
```
git commit -m "feat: added registration page"
```

6. Push your branch

```
git push origin feat/registration-page
```

8. Open a Pull Request (PR)
Target branch: testing.

9. After PR is merged
Delete your feature branch.
✅ Congrats, you’ve completed your first pull request!

Flow of Merging
- All changes go into the testing branch.
- Pull requests are reviewed and approved by Aisha.
- Share the PR link with Aisha for approval.
- Always include screenshots of UI changes or relevant code snippets.

Merging should follow this path:
```
feature branch -> testing branch -> develop branch -> main branch
```


```
 [feature/my-task] 
         |
         v
     [testing]
         |
         v
     [develop]
         |
         v
      [main]
⚠️ Important: Never force push to any branch.
```

### SSH Setup
Configure Git
```
git config --global user.name "your-username"
git config --global user.email "your-email@example.com"
```

Generate SSH key (if not done yet)
```
ssh-keygen -t ed25519 -C "your-email@example.com"
```
Test SSH connection
```
ssh -T git@github.com
```
🎉 Done!
kabalo nakag Git basics for this project:
Keep your commits clear
Keep your branches clean

Keep your pull requests focused
