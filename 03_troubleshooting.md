# Troubleshooting Sheet

## Problem: The commit button does not work
Check:
- Did you save the file?
- Did you write a commit message?
- Did you stage the file if your setup requires staging first?

## Problem: No changed files appear in Source Control
Check:
- Are you editing a file inside the repository folder?
- Did you save the file?
- Did you open the correct folder in VS Code?

## Problem: Push fails
Check:
- Are you signed in to GitHub?
- Do you have permission to the repository?
- Is internet access working?
- Read the exact error message in VS Code

## Problem: Pull changes do not appear
Check:
- Did the file really change on GitHub?
- Are you on the correct branch?
- Did pull complete successfully?
- Open the changed file again after pulling

## Problem: I changed the wrong branch
Check the branch name in the lower bar of VS Code.
Switch to the correct branch before continuing.

## Problem: Git says there is a conflict
Read the message carefully.
Open the conflicted file in VS Code.
Choose which version to keep, or combine both versions.
Then save, complete the merge, and commit if needed.

## Problem: I do not know what happened
Use this recovery sequence:
1. Stop making new changes
2. Read the current branch name
3. Open Source Control
4. Read the latest Git message in VS Code
5. Ask for help only after checking those four things
