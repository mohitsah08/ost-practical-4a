# Open Source Technologies - Practical 4.a

## Practical Title

Git Branching and Merging

## Objective

To understand Git branching, modifying files in a feature branch, committing changes, switching to the main branch, merging the feature branch, pushing the merged changes to GitHub, deleting the merged feature branch, and viewing Git history.

## Commands Performed

1. `git clone`
2. `cd`
3. `git branch`
4. `cat sample.txt`
5. `git switch -c feature-update`
6. `git branch`
7. `notepad sample.txt`
8. `cat sample.txt`
9. `git add sample.txt`
10. `git commit -m "Updated sample.txt in feature branch"`
11. `git switch main`
12. `cat sample.txt`
13. `git merge feature-update`
14. `cat sample.txt`
15. `git push origin main`
16. `git branch -d feature-update`
17. `git log --oneline`

## Repository

https://github.com/mohitsah08/ost-practical-4a

## Branching Workflow

```
main
  |
  +--- feature-update
          |
          +--- modify sample.txt
          |
          +--- commit
  |
  +--- merge feature-update
  |
  +--- push main
  |
  +--- delete feature-update
```

## Screenshots Included

The `screenshots/` directory contains complete visual verification of all practical steps:

- `01_clone_repository.png`: Cloned GitHub repository and entered directory.
- `02_initial_branch.png`: Checked initial active branch (`main`).
- `03_initial_sample_content.png`: Inspected initial content of `sample.txt`.
- `04_create_feature_branch.png`: Created and switched to branch `feature-update`.
- `05_modified_sample_file.png`: Modified `sample.txt` and verified added line.
- `06_git_add_status.png`: Staged changes and verified `git status`.
- `07_feature_commit.png`: Committed changes with message `"Updated sample.txt in feature branch"`.
- `08_switch_to_main.png`: Switched back to `main` branch.
- `09_before_merge_main_content.png`: Verified pre-merge state (feature changes not yet present on `main`).
- `10_merge_feature_update.png`: Merged `feature-update` into `main` and verified content.
- `11_push_to_github.png`: Pushed updated `main` branch to remote GitHub repository.
- `12_github_repository.png`: Browser view of GitHub repository reflecting updated files and commits.
- `13_delete_feature_branch.png`: Deleted merged `feature-update` branch and verified with `git branch`.
- `14_git_log.png`: Displayed compact Git log and graph showing full history.
