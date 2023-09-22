# Docker Desktop For Windows Junction Issue Reproducer

### Steps To Reproduce
1. [_Create a Directory Junction_](https://bit.ly/mklinkSyntax) ***from*** a Windows file system directory located on a partition of an internal disk drive (`SOURCE`) ***to*** a directory located on a ***removable*** drive  (`DESTINATION`)
2. Download and extract this reproducer project
3. Edit the `.env` file found at the root of this reproducer with appropriate values for `SOURCE` and `DESTINATION` on your own workstation
4. In a Windows command shell¹ (_cmd, PowerShell, Git Bash for example_), run: `docker compose up`

<br />
<br />
<br />
<br />
———
<br />

¹ The volume is successfully created if `docker compose up` is ran in a WSL 2 shell.