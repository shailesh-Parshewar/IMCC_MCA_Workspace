# Python — Semester 1

Welcome to the Python coursework directory for MCA students at IMCC!

This directory is for Python assignments, practicals, exercises, and personal practice related to the Semester 1 syllabus.

## 📁 Directory Structure

Every student must maintain a separate directory inside the Python directory.

```text
Python/
├── README.md
├── Shailesh-Parshewar/
│   ├── basics.py
│   ├── loops.py
│   ├── functions.py
│   └── assignments/
│       └── assignment-1.py
└── Student-Name/
    └── ...
```

Replace `Student-Name` with your own name, matching your student branch name.

## 🐍 What Can You Contribute?

You can add work related to:

- Python fundamentals, variables, and data types
- Conditional statements and loops
- Functions and recursion
- Lists, tuples, sets, and dictionaries
- String manipulation and file handling
- Object-oriented programming
- Practical assignments and programming exercises

Keep your files organized and use descriptive filenames.

## 🌿 Branching Workflow

Each student has a persistent student branch named after themselves. Subject branches are used to work on individual subjects before merging the changes into the student branch.

For example:

```text
semester-1
    └── Shailesh-Parshewar       ← Student branch
            └── Python           ← Local subject branch
```

The branch names illustrate the workflow; Git branches are not physically nested.

### Example: Adding a Python exercise

Suppose you want to add a program that checks whether a number is prime.

1. Switch to your student branch.
2. Create or switch to your local `Python` subject branch.
3. Add your file inside `Python/Your-Name/`.
4. Commit your changes.
5. Merge the subject branch into your student branch.
6. Push your student branch and open a pull request targeting `semester-1`.

Example file location:

`Python/Shailesh-Parshewar/prime_number.py`

Example program:

```python
def is_prime(number: int) -> bool:
    if number < 2:
        return False

    for divisor in range(2, int(number**0.5) + 1):
        if number % divisor == 0:
            return False

    return True


number = int(input("Enter a number: "))
print(is_prime(number))
```

This is only an example of how to organize your work. You should submit your own solutions and exercises.

## 📝 Contribution Guidelines

- Keep all your work inside your own student directory.
- Use meaningful filenames, such as `prime_number.py` or `list_operations.py`.
- Include comments where they help explain your approach.
- Do not modify another student's files without permission.
- Do not push your local subject branches to the central repository.
- Submit contributions through a pull request targeting `semester-1`.
- **Do not delete your student branch after a pull request is merged.** You will reuse it for future coursework.

For the full workflow, read the repository's `CONTRIBUTING.md`.

Happy coding! 🚀
