# useful-development-bash-commands
Just a collection of useful commands to use in terminals (mac/linux) when coding.

---

### Processes

##### Terminate process running on a port (mac/linux)
- Replace 3000 with the port the process is running on
- `lsof -ti :3000 | xargs kill -9`

---

### Git

##### Undo all uncommitted changes and go back to last commit
- `git reset HEAD --hard`

##### Remove differences between main and branch 'branch_A' from a third branch 'branch_B'
- Inside of *branch_B*: `git diff main branch_A | git apply -R`

##### List changed files between current branche and other branch
- `git diff --name-only other_branch`
  
---

### Browser

##### Freeze browser when trying to open tooltips/popups
- `setTimeout(() => { debugger; }, 3000);`
