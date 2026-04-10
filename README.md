# useful-development-bash-commands
Just a collection of useful commands to use in terminals (mac/linux) when coding.

#### Terminate process running on a port (mac/linux)
- Replace 3000 with the port the process is running on
- `lsof -ti :3000 | xargs kill -9`
