# MCA Students Repository — IMCC

A collaborative repository for MCA students at IMCC to maintain semester-wise coursework, practice programs, homework, and academic exercises while learning Git and GitHub collaboration.

## 🎯 Purpose

This repository is intended to help students:

- Maintain their coursework and programming practice in one place.
- Learn Git and GitHub workflows, including branching, commits, pushing, and pull requests.
- Share knowledge and learn from their classmates.
- Develop good collaboration habits through structured contributions.

## 📁 Repository Structure

Academic work is organized by semester, student, and subject.

```text
MCA-Students-Repository/
├── README.md
├── CONTRIBUTING.md
└── semester-1/
    ├── README.md
    ├── Shailesh-Parshewar/
    │   ├── Python/
    │   └── Data-Structures-Algorithms/
    └── Other-Student/
        ├── Python/
        └── Data-Structures-Algorithms/
```

The structure above illustrates the intended organization. Each student should use their own directory and keep their work inside the appropriate subject folder.

### Current subjects

- **Python**
- **Data Structures and Algorithms**

Additional subjects and semesters can be added as the programme progresses.

## 🌿 Branching Workflow

This repository uses a student-branch workflow to keep contributions organized.

1. **`main`** — Repository-wide documentation and contribution guidelines.
2. **`semester-1`** — The shared destination branch for Semester 1 coursework.
3. **Student branches** — Each student maintains a branch named after themselves, such as `Shailesh-Parshewar`.
4. **Subject branches** — Students can create local subject branches to work independently on each subject.

Subject branches are intended for local use or use within a student's own fork. They do not need to be pushed to the central repository.

### Example workflow

```text
semester-1
    │
    └── Shailesh-Parshewar
            ├── Python
            └── Data-Structures-Algorithms
```

The diagram represents the workflow conceptually. Git branches are not actually nested inside one another.

A typical contribution process is:

1. Start from the latest `semester-1` branch.
2. Create your student branch.
3. Create a local subject branch for the work you want to do.
4. Make changes inside your own student directory.
5. Commit your work on the subject branch.
6. Merge the subject branch into your student branch.
7. Push **only your student branch**.
8. Open a pull request targeting `semester-1`.

For detailed commands and rules, read [CONTRIBUTING.md](CONTRIBUTING.md).

## 🤝 Contribution Guidelines

Before contributing, please make sure you:

- Follow the required directory structure.
- Use your own student directory.
- Keep files in the appropriate subject folder.
- Write clear, meaningful commit messages.
- Avoid modifying another student's work without permission.
- Submit changes through a pull request rather than directly modifying protected branches.
- Follow any additional rules documented in `CONTRIBUTING.md`.

Pull requests may be reviewed before they are merged.

## 🔒 Repository Rules

Protected branches and repository permissions are intended to ensure that contributions are reviewed and the shared coursework remains organized.

Having access to the repository does not mean every branch can be modified directly. Follow the established contribution workflow and do not attempt to bypass branch protections.

## 📚 Getting Started

1. Make sure you have access to the repository.
2. Read [CONTRIBUTING.md](CONTRIBUTING.md).
3. Open the `semester-1` branch and read its `README.md`.
4. Set up your student branch and local subject branches according to the contribution guide.
5. Start adding your coursework in the appropriate directories.

## 💡 Remember

**One student, one student branch, one student directory.**

Keep subject work organized within your directory, use local subject branches to manage your work, and submit your student branch through a pull request to `semester-1`.

Happy coding! 🚀
