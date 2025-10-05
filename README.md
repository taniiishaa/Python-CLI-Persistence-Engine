# 🐍 Python-CLI-Persistence-Engine

[![Project Status](https://img.shields.io/badge/Status-Complete%20%7C%20Refactored-28a745?style=for-the-badge)](./todo.py)
[![Language](https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python)](./todo.py)
[![Focus](https://img.shields.io/badge/Focus-CLI%20Design%20%7C%20Data%20Integrity-007bff?style=for-the-badge)]()

---

## 💡 Project Overview: Robust Utility Development

This repository serves as a demonstration of foundational backend engineering principles applied to a **Command Line Interface (CLI)** environment. The core focus is not merely task management, but the effective implementation of a **Persistence Engine** to maintain data state across multiple user sessions using fundamental Python capabilities.

The included utility, a persistent To-Do list, is the functional output of this persistence engine design.

## 🛠️ Engineering Disciplines Demonstrated

This project showcases expertise in several crucial software development areas:

### 1. **Data Persistence and Integrity**
* **Decoupled Storage:** Implemented file I/O logic (`load_tasks`/`save_tasks`) completely separate from the application logic (CRUD operations), ensuring that the storage mechanism can be easily swapped (e.g., migrating from `.txt` to `SQLite`) without affecting the core UI or task logic.
* **Graceful Handling:** Included robust exception handling for `FileNotFoundError`, ensuring a clean boot process and initialization of the data store (`tasks.txt`) if it does not exist.

### 2. **Modular Architecture**
* **Separation of Concerns (SoC):** The application is broken down into small, single-responsibility functions (`add_task`, `remove_task`, `view_tasks`), making the codebase highly testable, readable, and maintainable.
* **Main Control Flow:** Utilizes the standard `if __name__ == "__main__":` entry point and a clear `main()` function with a persistent `while True` loop, reflecting a professional application structure.

### 3. **User Experience & Defensive Programming**
* **Input Validation:** Implemented explicit validation using `try...except ValueError` to handle non-integer input for menu choices and task numbers, preventing runtime crashes.
* **Clear Feedback Loop:** Provides instantaneous success/failure messages to the user for every operation (add, remove, invalid input).

---

## ⚙️ Application Structure

The entire application is contained within `todo.py` and manages a single data file: `tasks.txt`.

### Key Code Components:

| Function/Variable | Purpose | Engineering Highlight |
| :--- | :--- | :--- |
| `TASK_FILE` | Global constant for the data store name. | Uses constants for configuration, improving portability. |
| `load_tasks()` | Reads data from file into memory (`list`). | Manages file-not-found error gracefully. |
| `save_tasks()` | Writes data from memory back to file. | The core persistence writer. |
| `remove_task()` | Handles task deletion by index. | Includes logic for validating input against list boundaries. |

## 🚀 Quick Setup

This application requires only a standard Python environment.

1.  **Run the script:**
    ```bash
    python todo.py
    ```
2.  **Interact with the Menu:**
    Enter `1` to view, `2` to add, `3` to remove, and `4` to exit. Tasks will be saved in a new `tasks.txt` file in the same directory.

## 🎯 Outcome

This exercise successfully delivered a durable CLI utility, validating my ability to design and implement simple yet effective **data persistence and integrity layers** within a Python application. It showcases a commitment to **clean, modular, and defensible code** capable of serving as a boilerplate for future command-line tools.
