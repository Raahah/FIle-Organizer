
# File Organizer Script

This Python script organizes files in a specified directory into folders based on their file extensions. The script automatically creates folders for each file extension (if they don't already exist) and moves the files into the corresponding folders.



## How the Script Works:

**Input Path:**

The script prompts the user to input the path of the directory they want to organize.

**List Files:**

The script lists all files in the specified directory using os.listdir().

**Extract File Extension:**

For each file in the directory, the script extracts the file's extension using os.path.splitext().

**Check for Folder Existence:**

The script checks if a folder for the file extension already exists in the directory.
If the folder exists, the file is moved into it.
If the folder doesn't exist, the script creates the folder and then moves the file into it.

**Move Files:**

The script uses shutil.move() to move each file into its corresponding folder based on its extension.

**Output:**

After running the script, the specified directory will have subfolders named after file extensions (e.g., txt, jpg, pdf), and the files will be organized into these folders.

**Example Usage:**

Run the script.
Enter the path of the directory you want to organize (e.g., /Users/username/Desktop/MyFiles).
The script will organize the files into folders like txt, jpg, pdf, etc.



## Requirements:

Python 3.x
os and shutil modules (part of Python's standard library)

```bash
  This script assumes that the specified directory contains only files and no nested directories.
The script will skip files without an extension.
```
    