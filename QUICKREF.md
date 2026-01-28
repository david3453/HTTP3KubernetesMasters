# Quick Reference - Working Across Devices

## Daily Workflow

### Starting Work (on any device)

```bash
cd HTTP3KubernetesMasters
git pull origin main
```

### Ending Work Session

```bash
git add .
git commit -m "Brief description of what you did"
git push origin main
```

## Essential Git Commands

| Command | Purpose |
|---------|---------|
| `git pull origin main` | Get latest changes from GitHub |
| `git status` | See what files changed |
| `git add .` | Stage all changes for commit |
| `git commit -m "message"` | Commit changes locally |
| `git push origin main` | Upload changes to GitHub |
| `git log --oneline` | View commit history |

## Switching Devices

**Scenario**: You worked on your Windows laptop, now moving to your stationary PC.

**On Windows Laptop** (end of session):
```bash
git add .
git commit -m "Implemented HTTP/3 server basics"
git push origin main
```

**On Stationary PC** (start of session):
```bash
git pull origin main
# Continue working with all your latest changes
```

## Common Scenarios

### Made Changes But Forgot to Commit

```bash
git stash                 # Save changes temporarily
git pull origin main      # Get latest changes
git stash pop            # Restore your changes
# Resolve any conflicts if needed
git add .
git commit -m "Your changes"
git push origin main
```

### Want to Try Something Experimental

```bash
git checkout -b experiment/my-test
# Make experimental changes
git add .
git commit -m "Experimental feature"
git push origin experiment/my-test
# Later, merge if successful or just switch back to main
```

### Check What Changed

```bash
git diff                    # See unstaged changes
git diff --staged          # See staged changes
git log --oneline -5       # See last 5 commits
```

## Tips

✅ **DO:**
- Pull before starting work each time
- Commit frequently with clear messages
- Push at the end of each session
- Use descriptive commit messages

❌ **DON'T:**
- Forget to pull before starting
- Leave uncommitted changes when switching devices
- Use vague commit messages like "update" or "fix"

## IDE Setup

If using VS Code, install:
- EditorConfig extension (for consistent formatting)
- GitLens (for enhanced Git features)

## Getting Help

Run `git status` at any time to see what state your repository is in.

For more details, see:
- [SETUP.md](SETUP.md) - Full setup instructions
- [CONTRIBUTING.md](CONTRIBUTING.md) - Development guidelines
