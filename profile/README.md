## About This Repository

This organization serves as the central hub for all code created and maintained within our codebase. It includes tools, scripts, pipelines, prototypes, and production components used across projects. Whether you're building something experimental or contributing to a core library, all repositories here follow the same structure and standards to ensure smooth collaboration, version control, and reuse.

To maintain consistency and avoid confusion, we enforce a clear and simple naming convention for all repositories and encourage good Git practices when working on shared code.

---

## Repository Naming Convention

All repositories must use the following naming format:

### Format:

**all-lowercase-with-dashes**

### Examples:

| Incorrect             | Correct                 |
| --------------------- | ----------------------- |
| `ReviewIDGenerator`   | `review-id-generator`   |
| `ProductMatchingTool` | `product-matching-tool` |
| `CXToolkit`           | `cx-toolkit`            |

### Naming Guidelines:

* Use only **lowercase letters**.
* Use **dashes** (`-`) to separate words.
* Avoid camelCase, PascalCase, underscores (`_`), or capital letters.
* Choose names that are **concise yet descriptive**, reflecting the repository’s purpose.
* Do not use prefixes like `repo-` or suffixes like `-tool` unless necessary for clarity.

### Rationale:

* Ensures compatibility across case-sensitive filesystems.
* Aligns with GitHub’s URL and search conventions.
* Makes typing and navigating in the command line easier.
* Improves clarity in documentation, scripts, and automated tools.

---

## Git Best Practices

When working in these repositories, please keep the following in mind:

### 1. **Cloning and Remotes**

* After renaming a GitHub repo, remember to update the remote in your local copy:

  ```bash
  git remote set-url origin https://github.com/yourusername/repo-name.git
  ```

### 2. **Branching**

* Use clear, descriptive branch names such as `feature/review-matching`, `fix/null-pointer`, or `refactor/input-parser`.
* Avoid working directly on `main` or `master`. Always use feature branches.

### 3. **Commits**

* Write meaningful commit messages. Start with a verb in the imperative form (e.g., `add review ID generator`, `fix data parsing bug`).
* Make small, focused commits rather than bundling unrelated changes.

### 4. **Pull Requests**

* Always create a pull request for team review.
* Add a short but informative description of what the PR does and why.

### 5. **Merging**

* Prefer **squash and merge** or **rebase and merge** to keep history clean (based on team preference).
* Avoid merge commits unless coordinating large or complex branches.

### 6. **Submodules and Dependencies**

* Avoid Git submodules unless explicitly required. If used, document their purpose and usage.
* Use `.gitignore` files to prevent committing large or sensitive files.

### 7. **Avoid Force Pushes**

* Never use `git push --force` on shared branches unless explicitly discussed and agreed upon by the team.
