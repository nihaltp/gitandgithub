# Git and GitHub Basics Practice

This project is for learning and practicing the **basic Git + GitHub contribution flow**.

If you are new to Git, follow the steps below from start to finish.

## Goal

- Clone a repository
- Fork it on GitHub
- Work on your own branch
- Open pull requests
- Sync and handle merge conflicts when needed

## Practice Flow

### 1) Clone this repository

```bash
git clone https://github.com/nihaltp/gitandgithub.git
cd gitandgithub
```

### 2) Fork this repository on GitHub

Use the **Fork** button on the GitHub website to create your own copy.

### 3) Add your fork as a new remote

Replace `<your-username>` with your GitHub username:

```bash
git remote add fork https://github.com/<your-username>/gitandgithub.git
git remote -v
```

### 4) Create a new branch and switch to it

```bash
git checkout -b add-<your-username>
```

### 5) Add a file about yourself

Create a file in `/participants` using your username, for example:

`participants/<your-username>.md`

You can use the format shown in:

`participants/template.md`

### 6) Commit and push your branch

```bash
git add participants/<your-username>.md
git commit -m "Add participant profile for <your-username>"
git push -u fork add-<your-username>
```

### 7) Create a Pull Request on GitHub

Open a PR from your fork branch (`add-<your-username>`) to this repository’s default branch.

### 8) After your PR is merged, update `files.txt`

Add your participant file path to `/files.txt`, for example:

`participants/<your-username>.md`

Commit and push again from a new branch.

### 9) Create another PR for `files.txt`

If GitHub shows merge conflicts, pull the latest changes, resolve conflicts, commit, and push again.

## Notes

- Keep each PR small and focused.
- Use meaningful commit messages.
- If you get stuck on conflicts, ask for help and share the exact error.