# Data Structures and Algorithms — Semester 1

Welcome to the Data Structures and Algorithms coursework directory for MCA students at IMCC!

Use this directory for DSA assignments, implementations, problem-solving exercises, and algorithm practice.

## 📁 Directory Structure

Every student must maintain a separate directory inside this subject directory.

```text
Data-Structures-Algorithms/
├── README.md
├── Shailesh-Parshewar/
│   ├── arrays/
│   │   └── array_operations.py
│   ├── searching/
│   │   └── binary_search.py
│   ├── sorting/
│   │   └── bubble_sort.py
│   └── linked_lists/
│       └── singly_linked_list.py
└── Student-Name/
    └── ...
```

Replace `Student-Name` with your own name, matching your student branch name.

You may organize your files by topic, assignment, or practical, as long as your directory remains organized.

## 🧠 What Can You Contribute?

You can add implementations and exercises involving:

- Arrays and strings
- Searching and sorting algorithms
- Linked lists
- Stacks and queues
- Trees and graphs
- Recursion and backtracking
- Hash tables and other data structures
- Algorithm analysis and time complexity
- Problem-solving exercises and practical assignments

Use clear filenames and organize related implementations together.

## 🌿 Branching Workflow

Each student has a persistent student branch named after themselves. Subject branches are used to work on individual subjects before merging the changes into the student branch.

For example:

```text
semester-1
    └── Shailesh-Parshewar       ← Student branch
            └── Data-Structures-Algorithms
                                    ↑
                            Local subject branch
```

The diagram illustrates the workflow, not a literal Git branch hierarchy.

### Example: Adding a binary search implementation

Suppose you want to implement binary search.

1. Switch to your student branch.
2. Create or switch to your local `Data-Structures-Algorithms` subject branch.
3. Add the implementation inside your student directory.
4. Commit your changes.
5. Merge the subject branch into your student branch.
6. Push your student branch and open a pull request targeting `semester-1`.

Example file location:

`Data-Structures-Algorithms/Shailesh-Parshewar/searching/binary_search.py`

Example implementation:

```python
def binary_search(values: list[int], target: int) -> int:
    left, right = 0, len(values) - 1

    while left <= right:
        middle = (left + right) // 2

        if values[middle] == target:
            return middle
        if values[middle] < target:
            left = middle + 1
        else:
            right = middle - 1

    return -1
```

Binary search requires the input list to be sorted. The function returns the index of the target, or `-1` if it is not found.

This example demonstrates the expected organization and style. You should submit your own work and exercises.

## 📝 Contribution Guidelines

- Keep all your work inside your own student directory.
- Organize implementations by topic or assignment.
- Use descriptive filenames and explain non-obvious logic.
- Where useful, include test cases and document assumptions.
- Do not modify another student's files without permission.
- Do not push your local subject branches to the central repository.
- Submit contributions through a pull request targeting `semester-1`.
- **Do not delete your student branch after a pull request is merged.** You will reuse it for future coursework.

For the full workflow, read the repository's `CONTRIBUTING.md`.

Keep solving, learning, and improving! 💻
