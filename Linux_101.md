# Beginner-Friendly Linux Command Tutorial

A simple, dynamic tutorial for beginners. Use this as a reference for common Linux file operations, SSH, and basic text processing.

---

## Section 1: Create and Delete Directories

### Create a directory

```bash
mkdir my_folder
```

Create multiple folders:

```bash
mkdir folder1 folder2
```

Create nested folders:

```bash
mkdir -p parent/child/grandchild
```

### Delete a directory

Delete an empty directory:

```bash
rmdir my_folder
```

Delete a directory with contents:

```bash
rm -r my_folder
```

Force delete:

```bash
rm -rf my_folder
```

---

## Section 2: Create Files

Create an empty file:

```bash
touch file.txt
```

Create and write to a file:

```bash
echo "Hello, World!" > hello.txt
```

Append to a file:

```bash
echo "New line" >> hello.txt
```

---

## Section 3: List Files (with Time Info)

Basic list:

```bash
ls -l
```

Human-readable sizes:

```bash
ls -lh
```

Sort by time:

```bash
ls -lt
```

List all (including hidden files):

```bash
ls -la
```

---

## Section 4: Copy Files and Directories

Copy a file:

```bash
cp source.txt backup.txt
```

Copy a directory:

```bash
cp -r folder1/ folder_copy/
```

---

## Section 5: SSH into a Remote Server (HPC)

Basic SSH:

```bash
ssh username@hpc.address
```

With GUI forwarding:

```bash
ssh -X username@hpc.address
```

---

## Section 6: Copy Files from HPC

### Using `scp`

From HPC to local:

```bash
scp username@hpc.address:/path/to/file.txt .
```

From local to HPC:

```bash
scp file.txt username@hpc.address:/remote/path/
```

### Using `rsync`

Efficient recursive copy:

```bash
rsync -av username@hpc.address:/remote/folder/ ./local_folder/
```

---

## Section 7: Check Number of Lines in a File

```bash
wc -l file.txt
```

---

## Section 8: Find a File in a Directory

Search by exact name:

```bash
find . -name "file.txt"
```

Search for all `.txt` files:

```bash
find . -name "*.txt"
```

---

## Section 9: Search for String in File Using `grep`

Basic search:

```bash
grep "keyword" file.txt
```

Ignore case:

```bash
grep -i "keyword" file.txt
```

Show line numbers:

```bash
grep -n "keyword" file.txt
```

---

## Section 10: Count Lines, Words, and Characters

```bash
wc file.txt
```

Just lines:

```bash
wc -l file.txt
```

---

## Section 11: View Beginning or End of a File

First N lines (default 10):

```bash
head file.txt
```

First 20 lines:

```bash
head -n 20 file.txt
```

Last N lines:

```bash
tail file.txt
```

Last 50 lines:

```bash
tail -n 50 file.txt
```

---

Happy Learning!

