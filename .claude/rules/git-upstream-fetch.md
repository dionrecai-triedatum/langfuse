# Git upstream fetch/pull rules

When pulling or fetching from the `upstream` remote:

- Only fetch/pull the `main` branch — never fetch all branches.
- Always pass `--no-tags` to avoid pulling in upstream's tags.

Examples:

```bash
git fetch upstream main --no-tags
git pull upstream main --no-tags
```

Do not run bare `git fetch upstream` or `git pull upstream` without
specifying `main` and `--no-tags`.
