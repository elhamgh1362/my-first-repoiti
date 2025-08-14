# my-# auto_task.py

import os

file_name = "task_file.txt"
content = """This is an automated file.
After creation, its content will be read and displayed."""

# Create the file if it does not exist
if not os.path.exists(file_name):
    with open(file_name, "w", encoding="utf-8") as f:
        f.write(content)
    print(f"File '{file_name}' has been created.")

# Read and print the content
with open(file_name, "r", encoding="utf-8") as f:
    data = f.read()
    print("\nFile content:")
    print(data)
first-repoiti
