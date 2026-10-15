# MCA Students Repository — IMCC

A collaborative repository for MCA students at IMCC to organize coursework, practice programming, and collaborate on academic work while learning Git and GitHub.

## 🎯 Purpose

This repository is intended to help students:

- Keep their academic work and programming practice organized.
- Learn Git and GitHub workflows, including branching, commits, pushing, and pull requests.
- Collaborate with classmates and learn from one another.
- Develop good version control and contribution habits.
- Maintain work related to semester subjects and the Value Added Course.

## 📚 Repository Scope

The repository supports work related to:

- **Semester coursework** — Programs, assignments, exercises, and other academic work.
- **Value Added Course** — An overview of a wide range of programming and software development topics, including practical exercises and learning activities.

The Value Added Course covers multiple areas of software development at an introductory or overview level. Contributions should reflect the topics covered during the course without requiring the repository to be organized around an exhaustive list of technologies.

## 📁 Repository Structure

Academic work is organized by semester, with student contributions maintained within the appropriate subject or course directories.

The repository also contains general documentation, including this README and the contribution guidelines.

For the exact directory structure and instructions on where to place your work, refer to the README on the relevant semester branch and the `CONTRIBUTING.md` file.

## 🌿 Branching Workflow

The repository uses a student-branch workflow to keep contributions organized and ensure that changes are reviewed before being added to the shared coursework.

The main branches have the following purposes:

- **`main`** — Contains repository-wide documentation and contribution guidelines.
- **Semester branches** — Contain shared coursework and the corresponding student directories.
- **Student branches** — Persistent branches maintained by individual students for their contributions.
- **Subject or course branches** — Local working branches that students can use to organize work before merging it into their student branch.

Git branches are independent references to commits, not directories nested inside one another. The branching structure describes the intended workflow rather than a literal hierarchy.

### Example Git workflow

Suppose your student branch is named `Your-Name` and you want to work on a particular course.

1. Start from the latest semester branch.
2. Create or switch to your student branch.
3. Create a local working branch for the course.
4. Make your changes and commit them.
5. Merge the working branch into your student branch.
6. Push your student branch to the repository or your fork.
7. Open a pull request targeting the relevant semester branch.

For example, the workflow can be represented as:

```text
semester-1
    └── Your-Name
          └── Local course branch
```

This diagram is conceptual; Git does not create branches inside other branches.

**Important:** Your student branch is intended to be reused for future contributions. Do not delete it after a pull request has been merged. Before starting subsequent work, update your local branches with the latest changes from the semester branch.

For the exact commands, fork instructions, and contribution procedure, read `CONTRIBUTING.md`.

## 🤝 Contribution Guidelines

Before contributing, please make sure you:

- Follow the prescribed directory structure.
- Keep your work inside your own student directory.
- Place files in the appropriate course or subject directory.
- Write clear, meaningful commit messages.
- Avoid modifying another student's work without permission.
- Submit contributions through pull requests instead of pushing directly to protected branches.
- Follow the rules documented in `CONTRIBUTING.md`.

Pull requests may be reviewed before they are merged.

## 🔒 Repository Rules

Protected branches and repository permissions help keep shared coursework organized and ensure that contributions are reviewed.

Repository access does not imply permission to push directly to every branch. All students are expected to follow the established contribution workflow and respect branch protections.

## 🚀 Getting Started

1. Make sure you have access to the repository.
2. Read `CONTRIBUTING.md` before making changes.
3. Switch to the appropriate semester branch and read its README.
4. Set up your student branch and any local working branches according to the contribution guide.
5. Add your work in the appropriate directory.
6. Submit your changes through a pull request.

## 💡 Remember

**Keep your work organized, use your student branch consistently, and contribute through pull requests.**

The goal is not only to maintain coursework but also to build practical Git and GitHub collaboration skills that will be useful in future projects.

Happy coding! 🚀
