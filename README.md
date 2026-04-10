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

##### Remove differences between main and branch 'A' from a third branch 'B'
- Inside of *branch_b*: `git diff main branch_a | git apply -R`
