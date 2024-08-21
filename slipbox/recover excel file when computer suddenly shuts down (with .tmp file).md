---
created_at: 2024-08-21
tags:
  - "#problem_solution"
  - "#excel"
---
## Problem Description

The problem occurred due to a power outage, which caused the computer to shut down with the file open in [[excel]].

## Reasoning Steps

1. I tried to open the `.xlsx` file, but excel warned that the file was corrupted.
2. I remembered that when excel opens a file to edit it creates a temporary file `.tmp`
3. So I searched in [[google]] if there is a way to recover de corrupted file with this `.tmp` file, and I found this [[#^ce72b8|link]]
4. And i discovered that this file is basically a `.xlsx` and tried to open it with [[excel]]
5. So there is the solution

## Solution Steps

1. Open [[excel]] normally, click to `Open` a file and search the corrupted file in the dialog
2. Change the option `Open` option to `Open and Repair`
3. So save this new file normally after this

## References

1. [.tmp file replaces original Excel file after editing](https://www.dropboxforum.com/t5/Delete-edit-and-organize/tmp-file-replaces-original-Excel-file-after-editing/td-p/737767) ^ce72b8