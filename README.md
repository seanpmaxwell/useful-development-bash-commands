# Useful Development Commands
Just a collection of useful commands to use in terminals (mac/linux) when coding.

---

### Processes

##### `lsof -ti :"port number" | xargs kill -9` 
- Terminate process running on a port (mac/linux, i.e. `lsof -ti :3000 | xargs kill -9`)

---

### Git

##### `git reset HEAD --hard` 
- Undo all uncommitted changes and go back to last commit

##### `git diff "branch a" "branch b" | git apply -R` (inside of *"branch c"*)
- Remove differences between branch a and b from the branch you a currently in
- This is useful if you checkout c from b, when you mean to checkout c from a. 

##### `git diff --name-only "other branch"` 
- List changed files between current branch and another branch
  
---

### Browser

##### `setTimeout(() => { debugger; }, 3000);` 
- Freeze the browser after 3 seconds
- Useful when trying inspect tooltips/popups in developer tools.
