# Contributing Guidelines

Welcome to the MCA Students Repository for IMCC!

This document explains how to organize your work, use branches correctly, and submit contributions through pull requests. Please read these guidelines before contributing.

## 1. Core Rules

Before you begin, understand these four rules:

1. **One student, one student branch.** Use your name for your student branch, for example, `Shailesh-Parshewar`.
2. **One subject, one directory.** Each subject has its own directory inside the semester branch.
3. **One student directory per subject.** Store your work inside your own directory under the relevant subject.
4. **Submit through pull requests.** Do not push directly to protected shared branches or bypass the review process.

Your branch is used to manage your contributions. Your directory is where your submitted files live after merging.

## 2. Repository and Directory Structure

The repository is organized as:

```text
MCA-Students-Repository/
├── README.md
├── CONTRIBUTING.md
└── semester-1 (branch)
    ├── README.md
    ├── Python/
    │   ├── Shailesh-Parshewar/
    │   └── Student-Name/
    └── Data-Structures-Algorithms/
        ├── Shailesh-Parshewar/
        └── Student-Name/
```

The tree shows the contents of the `semester-1` branch. Student names are examples.

### Where should your files go?

| Subject | Your directory |
|---|---|
| Python | `Python/Your-Name/` |
| Data Structures and Algorithms | `Data-Structures-Algorithms/Your-Name/` |

Replace `Your-Name` with the name you use for your student branch.

**Do not create a student directory directly at the root of `semester-1`.** Your directory must be inside the relevant subject directory.

## 3. Understanding the Branch Structure

This repository uses the following branches:

- **`main`** — Repository-wide documentation and guidelines.
- **`semester-1`** — The shared branch containing subjects and merged student work.
- **Student branches** — Branches named after individual students, used to prepare contributions.
- **Subject branches** — Temporary or ongoing local branches used to work on individual subjects.

For example:

```text
semester-1
    │
    └── Shailesh-Parshewar       ← Student branch
            │
            ├── Python           ← Local subject branch
            └── Data-Structures-Algorithms
```

This diagram represents the workflow, not a literal hierarchy. Git branches are independent references; they are not nested folders.

Subject branches are intended to remain local or within your own fork. **Only push your student branch when submitting your work**, unless the repository maintainer explicitly instructs otherwise.

## 4. Setting Up Your Student Branch

First, clone the repository if you have not already done so:

```bash
git clone <repository-url>
cd <repository-folder>
```

Switch to the semester branch and update it:

```bash
git fetch origin
git switch semester-1
git pull origin semester-1
```

Create your student branch from the semester branch:

```bash
git switch -c Your-Name
```

For example:

```bash
git switch -c Shailesh-Parshewar
```

Use a consistent name for your student branch and your student directories. Check that a branch with your chosen name does not already exist in your local repository.

If you are contributing through your own fork, make sure your fork's `semester-1` branch is up to date before creating your student branch.

## 5. Creating and Using Subject Branches

Create a separate local branch for each subject you want to work on.

For example, to work on Python:

```bash
git switch Shailesh-Parshewar
git switch -c Python
```

Create your student directory if it does not already exist:

```bash
mkdir -p Python/Shailesh-Parshewar
```

Add your Python files inside that directory.

For another subject, switch back to your student branch and create another subject branch:

```bash
git switch Shailesh-Parshewar
git switch -c Data-Structures-Algorithms
```

Then add your files inside:

```text
Data-Structures-Algorithms/Shailesh-Parshewar/
```

**Important:** Create each subject branch from your student branch, not from another subject branch. This keeps subject work separate and makes it easier to merge your contributions.

If a subject directory already exists, use it rather than creating a duplicate or differently named directory.

## 6. Committing Your Work

Before committing, check your changes:

```bash
git status
```

Stage the relevant files and commit them:

```bash
git add .
git commit -m "Add Python practice exercises"
```

Use meaningful commit messages that describe what you changed.

Good examples:

- `Add Python loops exercises`
- `Implement binary search`
- `Add array operations`
- `Fix linked list traversal`

Avoid vague messages such as `update`, `changes`, or `final`.

## 7. Merging Subject Work into Your Student Branch

After finishing a subject task, switch back to your student branch:

```bash
git switch Shailesh-Parshewar
```

Merge the subject branch into it:

```bash
git merge Python
```

Repeat for each subject branch whose work you want to include.

Resolve any merge conflicts before continuing. Make sure the resulting files are in the correct `Subject/Your-Name/` directories.

Your student branch is now the branch that contains the combined work you intend to submit.

## 8. Pushing Your Student Branch

Before pushing, ensure that your student branch contains the latest semester changes where appropriate and that your work is committed.

If you have permission to push your student branch to the central repository:

```bash
git push -u origin Shailesh-Parshewar
```

If contributions must go through your own fork, push your student branch to your fork instead:

```bash
git push -u origin Shailesh-Parshewar
```

In the fork workflow, `origin` should point to your fork, while the original repository is typically configured as `upstream`.

**Do not push your local subject branches to the central repository.** The student branch is the contribution branch used for review.

## 9. Opening a Pull Request

Open a pull request on GitHub with these settings:

- **Base repository:** The shared MCA Students Repository, or the original repository if working through a fork.
- **Base branch:** `semester-1`.
- **Compare branch:** Your student branch, such as `Shailesh-Parshewar`.

In the pull request description, briefly explain:

- Which subjects you worked on.
- What you added or changed.
- Any relevant assignment or exercise details.

Review the changed-files list before submitting. Confirm that your files are inside the correct directories and that you have not accidentally included unrelated changes.

Wait for review and approval before expecting the contribution to be merged.

After merging, your work will be available in the shared repository under the relevant subject directory. For example:

```text
semester-1/
└── Python/
    └── Shailesh-Parshewar/
        ├── loops.py
        └── functions.py
```

The student directory remains in the shared semester branch even after the student branch is no longer needed.

## 10. Rules for Contributions

Please follow these rules:

- Contribute only to your own student directories unless you have permission to modify another student's work.
- Do not delete, rename, or overwrite another student's files without permission.
- Use the existing subject directory names exactly as they appear in the repository.
- Do not create unnecessary nested directories.
- Do not commit passwords, API keys, tokens, `.env` files, or other secrets.
- Avoid committing generated files, dependencies, or unrelated personal files.
- Keep your work relevant to the subject and explain your code where necessary.
- Do not force-push shared branches or attempt to bypass branch protection.
- Follow any additional instructions from the repository maintainer or faculty.

### Do Not Delete Your Student Branch

**Your student branch is meant to be reused for future contributions. Do not delete it after your pull request has been merged.**

You will continue using the same student branch for future assignments, practicals, and coursework.

For each new contribution:

1. Update your local `semester-1` branch with the latest changes.
2. Update your student branch with the latest `semester-1` changes.
3. Create a new local subject branch for your next task, or reuse an existing one if appropriate.
4. Commit your work and merge the subject branch back into your student branch.
5. Push your student branch and open another pull request targeting `semester-1`.

The student branch is your ongoing contribution branch, not a temporary branch for a single pull request.

You may delete temporary subject branches after merging their work into your student branch if you no longer need them.

## 11. Common Mistakes to Avoid

### Creating a student directory at the wrong level

Incorrect:

```text
semester-1/
└── Shailesh-Parshewar/
    └── Python/
```

Correct:

```text
semester-1/
└── Python/
    └── Shailesh-Parshewar/
```

### Creating a subject branch from another subject branch

Avoid building a chain of subject branches. Create each subject branch from your student branch.

### Opening a pull request against the wrong branch

Your pull request should target `semester-1`, not `main` or a local subject branch.

### Pushing every branch

Push your student branch for review. Keep subject branches local or in your own fork unless explicitly instructed otherwise.

### Assuming branches are directories

A branch name does not determine the directory structure. You must place files in the correct subject and student directories yourself.

## 12. Getting Help

If you are unsure about the directory structure, Git commands, merge conflicts, or pull request process, ask the repository maintainer before making changes that could affect shared work.

Thank you for contributing and helping build a useful learning resource for MCA students at IMCC!

**Learn, practice, contribute, and collaborate.** 🚀
