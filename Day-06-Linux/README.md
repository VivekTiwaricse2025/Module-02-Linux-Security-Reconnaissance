# Day 6 — Linux Fundamentals

## Aim
Practise basic Linux terminal usage, file and directory management, user information, permissions and process inspection.

## Concepts
- Linux is an open-source operating system used on desktops, servers and security platforms.
- The terminal accepts commands; the shell (for example Bash) interprets them.
- The file-system tree starts at `/`; `~` represents the current user's home directory.
- Users and groups control access to system resources.
- Processes are running instances of programs, each identified by a PID.

## Commands to practise
| Command | Purpose |
|---|---|
| `pwd` | Show current directory |
| `ls -la` | List files, including hidden files |
| `cd folder` | Change directory |
| `mkdir practice` | Create a directory |
| `touch notes.txt` | Create an empty file |
| `cat notes.txt` | Display a text file |
| `cp a.txt b.txt` | Copy a file |
| `mv a.txt b.txt` | Move or rename a file |
| `whoami` | Show current username |
| `id` | Show user and group IDs |
| `ls -l` | Inspect permissions |
| `chmod 640 notes.txt` | Set owner read/write, group read, others none |
| `ps aux` | List running processes |
| `man ls` | Read the manual for `ls` |

## Practical exercise
Run in your own Linux account or a trusted training VM:
```bash
cd ~
mkdir day6-practice
cd day6-practice
touch notes.txt
echo "My first Linux practical" > notes.txt
cat notes.txt
cp notes.txt backup.txt
ls -la
chmod 640 notes.txt
ls -l
whoami
id
ps aux
```

## Expected observations
- A `day6-practice` folder is created in your home directory.
- `notes.txt` contains the sentence entered above.
- `backup.txt` is a copy of `notes.txt`.
- `ls -l` displays the permissions on `notes.txt`.
- `whoami`, `id` and `ps aux` display local system information.

## Record your actual result
- Operating system / distribution: __________________
- Terminal used: __________________
- Commands completed: __________________
- Screenshot filenames: __________________
- Issue faced and solution: __________________

## Review questions
1. What is Linux?
2. What is the difference between a terminal and a shell?
3. Explain `pwd`, `ls` and `cd`.
4. How are `cp` and `mv` different?
5. What do read, write and execute permissions mean?
6. Explain `chmod 640`.
7. What is a process?
8. What information does `ps aux` show?

## Security practices
Use least privilege, keep software updated, use strong authentication, and never execute unknown commands with administrator privileges.
