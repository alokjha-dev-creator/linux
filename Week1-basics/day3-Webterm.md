# Day 3: WebTerm Practice 🐧

Completed the WebTerm tutorial: 14 missions, all cleared.


## Commands Practiced

| Command | What it does | Example |
|---|---|---|
| `mkdir` | Create a directory | `mkdir Software` |
| `touch` | Create an empty file | `touch Os.txt` |
| `echo` | Print or write text | `echo "Linux is a Kernel" > Os.txt` |
| `cat` | Display file contents | `cat Os.txt` |
| `>>` | Append to a file (no overwrite) | `echo "Linux for beginners" >> Os.txt` |
| `grep` | Search for text inside a file | `grep "Linux" Os.txt` |
| `find` | Search for files by name or type | `find . -type f` |
| `mv` | Move or rename a file | `mv Os.txt Software/` |

## Mission Flow

1. Created a directory and files
2. Wrote content into a file with `echo`
3. Read it back with `cat`
4. Added more lines with `>>`
5. Searched inside the file with `grep`
6. Found files with `find`
7. Moved a file to another location with `mv`

## Example Output

```
$ grep "Linux" Os.txt
Linux for beginners
Linux is a Kernel

$ find . -type f
./Linux-copy.txt
./Os.txt
```


## Key Takeaways

- `>` overwrites, `>>` appends
- `grep` searches **inside** files, `find` searches for **files**
- Repetition beats reading: type it, break it, fix it

## Next

- Day 3 lab: `cat`, `less`, `head`, `tail`, `wc`, `tail -f`, `nano`
- Then: users & permissions
