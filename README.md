# Group 1 Assignment 2.1

## How to clone the repository

Clone the repository to your local machine using Git:

```bash
git clone <repository-url>
cd <repository-folder>
```

Replace `<repository-url>` with the URL of your repository and `<repository-folder>` with the name of the cloned folder. Make sure you are copying the HTTPS and not the SSH if you are using a github token. 

## How to run the script

Make sure the repository folder contains a text file named `sample.txt`, because the script reads input from that file.

Run the script with Python:

```bash
python analyze_text.py
```

## What output to expect

The script prints a table with one row for each line in `sample.txt`.

The output columns are:

- `Line`: the line number
- `Chars`: the number of characters in the line, excluding leading and trailing whitespace
- `Uppercase`: the number of uppercase letters in the line
- `% Upper`: the percentage of characters in the line that are uppercase

Example output:

```text
Line    Chars   Uppercase   % Upper
1       12      2           16.67%
2       8       1           12.5%
```

