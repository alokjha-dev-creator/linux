# Linux Fundamentals 🐧

This file contains my beginner-level Linux command notes and practical examples.

The goal is to understand the Linux command line by practicing common commands for navigating the filesystem, creating and managing files and directories, reading and modifying file contents, and searching for information.

---

# 1. Navigation Commands

## pwd — Print Working Directory

Shows the directory I am currently working in.

```bash
pwd
Example:

/home/user
ls — List Files and Directories

Shows the files and directories in the current location.

ls

For more detailed information:

ls -l

The detailed output can show information such as permissions, ownership, size, and modification time.

cd — Change Directory

Used to move into another directory.

cd documents

Move one level back:

cd ..

Go to the home directory:

cd ~
2. Creating Directories and Files
mkdir — Make Directory

Creates a new directory.

mkdir projects

Example:

mkdir linux-practice
touch — Create a File

Creates an empty file.

touch notes.txt

Multiple files can also be created:

touch file1.txt file2.txt file3.txt
3. Writing and Reading Files
echo — Display or Write Text

Display text in the terminal:

echo "Hello Linux"

Write text into a file:

echo "Linux is interesting" > notes.txt

The > operator writes the output into the file.

If the file already contains information, > replaces the existing content.

cat — Read File Contents

Displays the contents of a file.

cat notes.txt

Example:

echo "I am learning Linux" > notes.txt
cat notes.txt

Output:

I am learning Linux
4. Appending Content
>> — Append to a File

The >> operator adds new content to the end of an existing file.

echo "Linux is useful" >> notes.txt

For example:

echo "First line" > notes.txt
echo "Second line" >> notes.txt
cat notes.txt

Output:

First line
Second line
Important Difference
>

overwrites existing content.

>>

appends content to the existing file.

5. Copying Files and Directories
cp — Copy a File

Copies a file from one location to another.

cp notes.txt notes-copy.txt

This creates a copy named:

notes-copy.txt
cp -r — Copy a Directory

The -r option means recursive.

It allows us to copy a directory together with the contents inside it.

cp -r projects projects-copy

This creates:

projects/
projects-copy/

with the contents of the original directory copied into the new directory.

6. Moving and Renaming
mv — Move or Rename

Move a file into another directory:

mv notes.txt documents/

Rename a file:

mv old-name.txt new-name.txt

The same command can also be used to rename directories.

7. Removing Files and Directories
rm — Remove a File

Removes a file.

rm notes-copy.txt

Be careful when using rm because the file normally does not go to a recycle bin.

rmdir — Remove an Empty Directory

Removes an empty directory.

rmdir old-folder

rmdir only works when the directory is empty.

8. Searching
grep — Search Text

grep searches for specific text inside files.

Basic syntax:

grep "word" filename

Example:

grep "Linux" notes.txt

This displays the lines inside notes.txt that contain the word Linux.

find — Find Files and Directories

find can be used to search for files and directories.

Find a file:

find . -name "notes.txt"

Find a directory:

find . -type d -name "projects"

Here:

.       = current directory
-name   = search by name
-type d = search for directories
9. Basic Command Practice

A simple practice sequence:

mkdir linux-practice
cd linux-practice
touch notes.txt
echo "Linux fundamentals" > notes.txt
cat notes.txt
echo "Learning Linux commands" >> notes.txt
cat notes.txt
cp notes.txt notes-copy.txt
ls -l
grep "Linux" notes.txt

This small sequence demonstrates how multiple Linux commands can work together.
