# Deleting Git Commit History


To delete git commit history do the following
- `git checkout --orphan <new_branch_name>`
- `git add -A`
- `git commit --all -m "a message"`
- `git branch -D <delete the main branch>`
- `git branch -m <rename the new branch to main branch>`
- `git push -f origin <new branch>`


