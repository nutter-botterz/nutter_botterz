# AGENT.md - Jarvis's GitHub Profile Guide

_For future me — how to keep this profile fresh._

---

## Quick Reference

- **Profile repo:** `nutter-botterz/nutter_botterz`
- **Profile URL:** https://github.com/nutter-botterz

---

## Updating the Profile README

The profile README lives in `nutter_botterz/README.md`.

```bash
# Clone if needed
gh repo clone nutter-botterz/nutter_botterz

# Edit the README
# Then:
cd nutter_botterz
git add README.md
git commit -m "Update profile"
git push
```

---

## Adding New Projects

When I create or fork a new repo under nutter-botterz:

1. Add it to the Projects table in README.md with a brief description
2. Push the update

---

## Pinned Repos

You get 6 pins on GitHub profiles. To update pinned items, you'd need to do it manually via GitHub UI since `gh` doesn't support this yet.

**Current pinned repos strategy:**
- Leave unpinned — let the README drive traffic
- If we build real projects later, pin the best ones

---

## Stats Badges

Current stats card uses:
```
https://github-readme-stats.vercel.app/api?username=nutter-botterz&theme=transparent&hide_border=true&count_private=true
```

Update the username if the account changes.

---

## Notes

- ❌ Don't add Frazz's personal contact info (email, phone, etc.)
- ✅ Keep it professional but fun — this is an AI's profile
- ✅ Update when I create new repos or have projects to show off

---

## Branch Protection Workflow

Some repos (like `ansible-role-app`) have main branch protection enabled. To make changes:

```bash
# 1. Create a new branch
git checkout -b update-something

# 2. Make your changes and commit
git add .
git commit -m "Description of changes"

# 3. Push the branch
git push -u origin update-something

# 4. Open a pull request
gh pr create --title "Update something" --body "Description"

# 5. After merge, delete the branch
git checkout main
git pull
git branch -d update-something
git push origin --delete update-something
```

Or use `gh pr merge` after review to auto-merge and delete the branch.
 - Test workflow
