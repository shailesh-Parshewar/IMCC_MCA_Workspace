# MCA Students Repository — IMCC

A collaborative repository for MCA students at IMCC to maintain semester-wise coursework, homework, and programming practice while learning Git and GitHub collaboration.

## 🎯 Purpose

This repository helps students:

- Maintain their academic work in an organized, shared space.
- Practice Git and GitHub, including branching, commits, pushing, and pull requests.
- Learn from classmates and share programming solutions.
- Develop good collaboration habits through code review and structured contributions.

## 📁 Repository Structure

The repository is organized by **semester, subject, and student**.

```text
MCA-Students-Repository/
├── README.md
├── CONTRIBUTING.md
└── semester-1/
    ├── README.md
    ├── Python/
    │   ├── Shailesh-Parshewar/
    │   └── Student-Name/
    ├── Data-Structures-Algorithms/
    │   ├── Shailesh-Parshewar/
    │   └── Student-Name/
    └── Networking-Fundamentals/
        ├── Shailesh-Parshewar/
        └── Student-Name/
```

The directory structure above represents the contents of the `semester-1` branch. The names shown are examples.

### Directory rules

- Each subject has its own directory.
- Inside each subject directory, every student has a separate directory.
- Students must store their work inside their own directory under the relevant subject.
- A student's directory remains in the shared repository after their pull request is merged.
- Do not create a student directory directly at the root of `semester-1`.

For example, Shailesh's Python work belongs in:

`Python/Shailesh-Parshewar/`

His Data Structures and Algorithms work belongs in:

`Data-Structures-Algorithms/Shailesh-Parshewar/`

## 🌿 Branch Structure

Branches are used to manage contributions; directories are used to organize files. These are two separate things.

The repository follows this workflow:

- **`main`** — Contains repository-wide documentation and contribution guidelines.
- **`semester-1`** — The shared branch containing Semester 1 subjects and merged student contributions.
- **Student branch** — Each student creates a branch using their own name, for example, `Shailesh-Parshewar`.
- **Subject branches** — Students create local branches to work on individual subjects before merging their changes into their student branch.

### Example branch workflow

```text
semester-1
    │
    └── Shailesh-Parshewar       ← Student branch
            │
            ├── Python           ← Local subject branch
            ├── Data-Structures-Algorithms
            └── Networking-Fundamentals
```

**Important:** Git branches are not physically nested. The diagram illustrates how branches are used in the workflow, not a literal branch hierarchy.

Subject branches are intended to remain local or within the student's own fork. Students should push only their student branch for submission to the shared repository.

## 🔄 Contribution Workflow

Each student should follow these steps:

1. Start from the latest `semester-1` branch.
2. Create a student branch using their name.
3. Create a local subject branch from their student branch.
4. Add or modify files inside the appropriate `Subject/Student-Name/` directory.
5. Commit the changes on the subject branch.
6. Merge the subject branch back into the student branch.
7. Push only the student branch to the central repository or their own fork, as permitted.
8. Open a pull request targeting `semester-1`.
9. Wait for review and approval before the pull request is merged.

After merging, the student's work will be available in the relevant subject directory on `semester-1`. The student branch is a contribution mechanism; the student directory is where the submitted work lives.

For commands and detailed rules, read [CONTRIBUTING.md](CONTRIBUTING.md).

## 🤝 Contribution Guidelines

Before contributing:

- Read `CONTRIBUTING.md` and the `semester-1/README.md`.
- Use your own student branch and student directory.
- Follow the existing subject and directory names.
- Write clear, meaningful commit messages.
- Do not modify another student's work without permission.
- Do not push directly to protected branches or bypass pull-request reviews.
- Keep your submissions relevant to the subject.

Pull requests may be reviewed before being merged.

## 🔒 Repository Rules

Protected branches and repository permissions are intended to keep the shared coursework organized and ensure contributions are reviewed.

Having repository access does not necessarily grant permission to push to every branch. Follow the contribution workflow and the configured GitHub branch rules.

## 🚀 Getting Started

1. Make sure you have access to the repository.
2. Read this README and [CONTRIBUTING.md](CONTRIBUTING.md).
3. Switch to `semester-1` and read its README.
4. Create your student branch and local subject branches according to the contribution guide.
5. Add your work to the appropriate `Subject/Student-Name/` directory.
6. Submit your student branch through a pull request targeting `semester-1`.

## 💡 Remember

**Branches manage your work; directories organize your submissions.**

- Student name = branch name.
- Subject = directory at the semester level.
- Student name inside a subject = directory containing that student's work.
- Pull request target = `semester-1`.

Happy coding! 🚀
