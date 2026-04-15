# Self-Paced Git Workshop Lab (90 minutes)

## Goal
By the end of this lab, you will be able to:
- make a commit in VS Code
- push changes to GitHub
- pull changes from GitHub to VS Code
- create a branch
- merge a branch into `main`

## What you need
- A GitHub account
- Git installed on your computer
- Visual Studio Code installed
- Access to your own GitHub repository for this workshop

## The simple model
Think of Git in four parts:
1. **Files on your computer**
2. **Staged changes** (changes selected for the next commit)
3. **Commit history** (saved checkpoints)
4. **GitHub remote** (the online copy of the repository)

## Before you start
You should already have a repository that contains these files:
- `README.md`
- `profile.txt`
- `hobby.txt`
- `weekend-plan.txt`

If your repository does not contain them, ask the teacher for the starter files.

---

## Part 1 - Open the repository in VS Code

### Task 1
Open your repository in VS Code.

If you already have the repository on your computer:
- Open VS Code
- Select **File > Open Folder**
- Open your repository folder

If you do not have the repository on your computer yet:
- Clone it from GitHub
- Open the cloned folder in VS Code

### Checkpoint
You should see:
- your project files in the Explorer
- a **Source Control** icon on the left side

---

## Part 2 - Make your first commit

### Task 2
Open `README.md` and add this section at the end:

```md
## Student information
Name: YOUR NAME
Group: YOUR GROUP
```

Replace `YOUR NAME` and `YOUR GROUP` with your own information.

Save the file.

### Checkpoint
Open **Source Control** in VS Code.
You should see `README.md` listed as a changed file.

### Task 3
Stage the change.

Then write this commit message:

```text
Add student information to README
```

Commit the change.

### Checkpoint
After the commit:
- the change list should become empty
- the repository should show 1 new local commit

---

## Part 3 - Push to GitHub

### Task 4
Push your commit to GitHub.

### Checkpoint
Open your repository on GitHub in the browser.
You should see the updated `README.md` and your commit in the history.

---

## Part 4 - Pull a change from GitHub

### Task 5
Now make a change directly in GitHub:
- Open `hobby.txt` in GitHub
- Click the pencil/edit button
- Replace the line `Main hobby:` with your own hobby
- Save the change directly in GitHub

Suggested text:

```text
Main hobby: walking in nature
```

### Checkpoint
GitHub now has one change that your local repository does not have.

### Task 6
Go back to VS Code and pull the latest changes from GitHub.

### Checkpoint
Open `hobby.txt` in VS Code.
You should see the text you edited in GitHub.

---

## Part 5 - Create and use a branch

### Task 7
Create a new branch called:

```text
add-weekend-plan
```

Switch to that branch.

### Checkpoint
VS Code should show that you are on branch `add-weekend-plan`.

### Task 8
Open `weekend-plan.txt` and replace its contents with this template:

```text
Weekend plan
- Saturday:
- Sunday:
```

Then add your own short plan.

Example:

```text
Weekend plan
- Saturday: visit family
- Sunday: go for a run
```

Save the file.

### Task 9
Stage the file and commit it with this message:

```text
Add weekend plan
```

### Task 10
Push the branch to GitHub.

### Checkpoint
Your branch and commit should now also exist on GitHub.

---

## Part 6 - Merge the branch into main

### Task 11
Switch back to branch `main`.

### Task 12
Merge branch `add-weekend-plan` into `main`.

### Task 13
Push `main` to GitHub.

### Checkpoint
On GitHub, branch `main` should now contain the `weekend-plan.txt` changes.

---

## Part 7 - Final check

You have completed the lab if you can answer **yes** to all of these:
- I opened a Git repository in VS Code. - yes
- I made a change locally. - yes
- I staged and committed that change. - yes
- I pushed a commit to GitHub. - yes
- I changed a file in GitHub and pulled it into VS Code. - yes
- I created a branch. - yes
- I committed on the branch. - yes
- I merged the branch into `main`. - yes

---

## Optional extension - Simple merge conflict

Do this only if you have completed everything above.

### Task A
Make sure you are on `main`.
Open `profile.txt` and change the line:

```text
Favorite drink: coffee
```

to:

```text
Favorite drink: tea
```

Commit the change on `main`.

### Task B
Switch to a new branch called `drink-change`.
Change the **same line** in `profile.txt` to:

```text
Favorite drink: water
```

Commit the change.

### Task C
Switch back to `main` and merge `drink-change`.

You should now get a merge conflict.
Resolve it in VS Code and choose the final text you want.
Then complete the merge and push the result.

---

## Good habits to remember
- Save files before staging and committing.
- Read the branch name before you make changes.
- Commit small changes with clear messages.
- Push after finishing a meaningful step.
- Pull before starting new work if the remote may have changed.
