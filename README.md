📌 Task Summary

- This repository contains a Command-Line Interface (CLI) To-Do List Application built using Python.
- The project was part of my internship tasks and helped me understand persistent data storage, user interaction in CLI, and modular program design.

🚀 My Development Process

1. Project Planning & Breakdown
- Defined the objective: build a simple task manager with add, view, and remove options.
- Planned persistence so tasks remain saved even after closing the program.
- Chose a list data structure for managing tasks in memory and a text file (tasks.txt) for storage.

2. Core Implementation
- Designed an interactive CLI menu using a while loop.
- Implemented modular functions for:
- Viewing tasks
- Adding tasks
- Removing tasks
- Saving/loading tasks from a file

3. File Handling & Persistence
- Used Python’s built-in open() method for reading/writing tasks.
- Stored tasks line by line in tasks.txt.
- Ensured tasks reload automatically each time the program starts.

4. Error Handling & User Experience
- Validated user input for correct menu selection.
- Added checks for invalid task numbers when removing tasks.
- Handled FileNotFoundError gracefully if tasks.txt doesn’t exist yet.

5. Collaboration & Deployment with GitHub
- Pushed the final code (todo.py) to GitHub.
- Documented the process and features clearly in this README file.

📖 Application Description

- This is a persistent, user-friendly CLI To-Do List Manager written in Python.
- It demonstrates fundamental programming concepts such as lists, loops, conditional logic, modular code structure, and file handling.
- The app helps users manage their tasks effectively from the terminal, ensuring that tasks are saved and accessible across multiple sessions.

✨ Key Features

- Simple & Interactive CLI – Intuitive text-based menu system.
- Task Management – Add, view, and remove tasks easily.
- Persistent Storage – Tasks are saved to tasks.txt and reloaded automatically.
- Error Handling – Prevents crashes from invalid inputs.
- User-Friendly – Clear prompts and instructions for smooth usage.

⚙️ Technologies Used

- Language: Python
- Tools: VS Code / Terminal

🎯 Outcome

- This project resulted in a persistent CLI-based To-Do App, showcasing my ability to:
- Build interactive Python applications
- Work with file handling for data persistence
- Apply modular coding practices
- Document and share code effectively using GitHub
