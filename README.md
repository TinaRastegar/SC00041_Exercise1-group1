# SC00041 Exercise 1 - Group 1

This repository contains a Python script that analyzes a text file and reports character counts and uppercase percentages for each line.

## Prerequisites

- Git installed on your computer
- Python 3 installed
- A text editor such as nano, VS Code, or similar

## Setup

### 1. Clone your repository

Open Terminal on your computer and run:

```bash
git clone https://github.com/TinaRastegar/SC00041_Exercise1-group1.git
```



### 2. Check that the files were downloaded

Run:

```bash
ls
```

You should see something like:

```bash
analyze_text.py
sample.txt
```

### 3. Test the script BEFORE changing anything

Run:

```bash
python3 analyze_text.py
```

You will likely get this error:

```bash
FileNotFoundError: [Errno 2] No such file or directory: '/home/user/Desktop/sample.txt'
```

This happens because the script uses an absolute file path that does not exist on your computer.

## Fix the script

### 4. Edit the file path

Open the script with a text editor:

```bash
nano analyze_text.py
```

Find this line:

```python
My_file = "/home/user/Desktop/sample.txt"
```

Change it to:

```python
My_file = "sample.txt"
```

Save the file and exit.

## Test the fix

### 5. Run the script again

```bash
python3 analyze_text.py
```

Expected output:

```bash
Line    Chars  Uppercase  % Upper
1       12     2          16.67%
2       15     8          53.33%
3       20     5          25.0%
```

## Git workflow

### 6. Create a new branch

```bash
git checkout -b fix-file-path
```

### 7. Stage and commit your changes

```bash
git add analyze_text.py
git commit -m "Fix file path to use local sample.txt"
```

### 8. Push the branch to GitHub

```bash
git push origin fix-file-path
```

### 9. Open a Pull Request

Go to the repository on GitHub and open a pull request from `fix-file-path` into the main branch.

### 10. Review and merge

After review, merge the pull request on GitHub.

## Notes

- Using a relative path like `sample.txt` makes the script portable.
- It is better to stage only the modified file instead of using `git add .`.
- The README should show both the expected error and the corrected output to make the exercise easier to follow.

