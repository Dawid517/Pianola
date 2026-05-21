# Commit Message Convention

This project follows a lightweight convention for commit
messages to keep history readable and make collaboration easier.

## Format

```text
<type>: <short description>
```

Example:

```text
feat: add motor driver abstraction
fix: correct UART baud rate
docs: update setup instructions
```

### Rules

- Use lowercase for the commit type
- Keep the description short and clear
- Use imperative mood (e.g. "add", not "added")
- Do not end descriptions with a period
- Keep the first line under ~72 characters
- One commit should represent one logical change

---

## Commit Types

### `feat`
New functionality or capability.

```text
feat: add PID controller
feat: implement CAN communication
```

---

### `fix`
Bug fixes.

```text
fix: correct battery voltage calculation
fix: prevent application crash on startup
```

---

### `docs`
Documentation changes only.

```text
docs: update README
docs: add firmware flashing guide
```

---

### `refactor`
Code restructuring without changing behavior.

```text
refactor: split sensor module
refactor: simplify state machine
```

---

### `style`
Formatting or style changes only.

```text
style: apply formatter
style: fix indentation
```

---

### `test`
Add or update tests.

```text
test: add UART integration tests
test: improve controller coverage
```

---

### `build`
Build system or dependency changes.

```text
build: update PlatformIO dependencies
build: configure GitHub Actions
```

---

### `ci`
Continuous integration changes.

```text
ci: add release workflow
ci: cache build artifacts
```

---

### `perf`
Performance improvements.

```text
perf: optimize image processing
perf: reduce memory usage
```

---

### `chore`
Maintenance tasks that do not affect application logic.

```text
chore: reorganize project folders
chore: remove unused assets
```

---

## Optional Scope

If useful, include a scope:

```text
<type>(<scope>): <description>
```

Examples:

```text
feat(firmware): add encoder support
fix(hardware): correct PCB net labels
docs(readme): clarify setup process
```

---

## Good Examples

```text
feat: add emergency stop logic
fix: prevent invalid sensor readings
docs: add architecture overview
refactor(control): simplify command flow
```

## Avoid

Too vague:

```text
update stuff
changes
fix bug
commit
```

Too broad:

```text
feat: rewrite entire project
```

Multiple unrelated changes (bad):

```text
fix: repair UART and update README and remove files
```

---

## Pull Requests

Before opening a PR:

- Squash unnecessary commits
- Ensure commit messages follow this convention
- Verify the project builds successfully
- Link related issue if applicable
