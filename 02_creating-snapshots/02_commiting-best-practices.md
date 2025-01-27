# Commiting best practices

## 1. Write Meaningful Commit Messages
   - Use an imperative tone: "Add user authentication" (not "Added" or "Adding").
   - Summarize the change in the first line (50 characters max).
   - Add an optional description below (separate with a blank line) if the change needs clarification or details.

   Example:
   ```
   Fix login redirect issue

   Update the authentication middleware to handle edge cases
   when users attempt to access restricted pages.
   ```

---

## 2. Commit Small and Logical Changes
   - Each commit should address a single purpose or change.
   - Avoid committing unrelated changes together (e.g., fixing a bug and updating documentation in the same commit).

---

## 3. Avoid Large Commits
   - Break down large changes into smaller, focused commits to make your history easier to review.
   - This also helps with debugging by isolating changes.

---

## 4. Test Before Committing
   - Ensure your changes work as expected before committing.
   - Avoid committing broken or half-implemented features unless it's part of a development branch.

---

## 5. Use .gitignore to Exclude Unnecessary Files
   - Avoid committing temporary files, logs, IDE settings, or other artifacts by configuring your `.gitignore` file properly.

---

## 6. Commit Frequently (But Not Excessively)
   - Commit after each meaningful unit of work, but don’t commit every single small edit or typo fix unless it’s critical.

---

## 7. Use Branches for Features or Bug Fixes
   - Work on a separate branch for new features, fixes, or experiments (e.g., `feature/login-page` or `bugfix/header-crash`).
   - Merge branches into the main branch (e.g., `main` or `develop`) after review.

---

## 8. Review Changes Before Committing
   - Use `git diff` or `git status` to review what you’re about to commit.
   - This ensures that only the intended changes are included.

---

## 9. Follow a Commit Message Convention
   - Use a standard format for consistency. For example, the Conventional Commits standard:
     ```
     feat: add user authentication
     fix: resolve login redirect issue
     docs: update README with setup instructions
     refactor: simplify error handling logic
     test: add tests for login functionality
     chore: update dependencies
     ```

---

## 10. Avoid Commiting Sensitive Data
   - Double-check to ensure API keys, passwords, or other sensitive information aren’t committed.

---

--
## 11. Avoid "WIP" or Placeholder Commits
   - Instead, use tools like `git stash` to temporarily save incomplete work without committing it.

---

## 12. Rebase Before Merging (If Necessary)
   - Use `git rebase` for a cleaner history when working on feature branches. Avoid rebasing public/shared branches.

---

## 13. Write Descriptive Commit History
   - Avoid vague messages like "Fix stuff" or "Update". These don’t provide meaningful context to others (or even your future self).
