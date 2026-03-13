# 📔 Personal Journal Manager: File Operator

A robust, object-oriented Python utility designed for secure and organized digital journaling. This application serves as a comprehensive guide to **File I/O operations**, **Exception Handling**, and **String Manipulation** in Python.

---

## 🌟 Key Features

* **Persistent Storage:** Automatically manages a local `.txt` file to store your thoughts across sessions.
* **Timestamped Entries:** Every entry is automatically prefixed with a precise `[YYYY-MM-DD HH:MM:SS]` timestamp.
* **Smart Search:** A keyword-based retrieval system that scans through historical entries to find specific memories or dates.
* **Safe Deletion:** Includes a "Wipe All" feature with a confirmation prompt to prevent accidental data loss.
* **Error Resilience:** Sophisticated `try-except` blocks handle common issues like `PermissionError` and `FileNotFoundError` gracefully.

---

## 🛠️ Technical Implementation

The script utilizes a modular **Manager Class** architecture to separate logic from the user interface:

| Component | Responsibility |
| --- | --- |
| **`JournalManager`** | Encapsulates all file operations including `open()`, `read()`, `write()`, and `os.remove()`. |
| **`add_entry`** | Uses "Append" mode (`a`) to preserve existing data while adding new content. |
| **`view_all`** | Implements "Read" mode (`r`) with encoding support for universal character compatibility. |
| **`find_item`** | Processes file data in "chunks" to maintain the relationship between timestamps and entry text. |
| **`wipe_all`** | Interfaces with the `os` module to physically delete the journal file from the disk. |

---

2. **Write Your First Entry:** Select **Option 1** and type your thoughts. The system handles the formatting.
3. **Review History:** Select **Option 2** to see a formatted list of all your past entries.
4. **Find Specific Moments:** Select **Option 3** and enter a keyword (e.g., "Work" or "2024") to filter your logs.

---

## 📋 Requirements

* **Python 3.x**
* **Standard Libraries:** `os`, `datetime`

---

## 👤 Author

**Aesha makrubiya**

---
