# Bash and Command Line Snippets

- to reload iTerm: `exec $SHELL -l`
- to kill a process:  `ps -ef | grep puma`
- to REALLY kill:  `kill -9 24838 (really stop!)`
- to find running process: `lsof -wni tcp:3000`
- to kill: `kill -9 PID` (number of running process)
- to find a file in the current directory by name: find . | grep participant
- to find a file in the home directory by name: find ~/ | grep participant Read more [here](http://askubuntu.com/questions/144698/find-a-file-using-the-terminal)
- to change a word in vim (ex: pick to s): `cw`
