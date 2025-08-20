# Student Management System (C++)

This is a simple **Student Record Management System** built in C++ using file handling.
It allows users to **add**, **view**, and **search** student records, storing data in a text file (`stuData.txt`).

---

## 📌 Features

* **Add Student Record**

  * Saves student roll number, name, father’s name, and address in a text file.
  * Records are appended so existing data remains intact.

* **View All Student Records**

  * Reads all stored records from `stuData.txt` and displays them in a formatted manner.

* **Search Student Record**

  * Searches by **roll number** and displays the student details if found.

* **Exit Option**

  * Cleanly exits the program.

---

## 📂 File Structure

```
StudentManagement/
│── main.cpp         # Source code
│── stuData.txt      # Auto-created text file to store student records
│── README.md        # Documentation
```

---

## 🛠️ How It Works

1. When the program starts, it shows a **menu**:

   ```
   ---------------------------
   1- Add Student Record
   2- View All Student Record
   3- Search Student Record
   4- Exit
   ---------------------------
   ```
2. The user selects an option:

   * `1` → Prompts input for new student details and saves them.
   * `2` → Displays all stored student records.
   * `3` → Prompts for a roll number and displays matching student record (if found).
   * `4` → Exits the program.

---

## 📝 Example `stuData.txt`

If two records are added:

```
101*Alice*Robert*New York
102*Bob*David*Los Angeles
```

Output when viewing records:

```
Student Roll Number :: 101
Student Name :: Alice
Student Father Name :: Robert
Student Address :: New York

Student Roll Number :: 102
Student Name :: Bob
Student Father Name :: David
Student Address :: Los Angeles
```

---

## 🚀 Compilation & Execution

### Using g++

```bash
g++ main.cpp -o student
./student
```

### Using MinGW on Windows

```powershell
g++ main.cpp -o student.exe
student.exe
```
## ✅ Future Improvements

* Add **delete** and **update** record options.
* Input validation (e.g., no empty names).
* GUI interface (e.g., FLTK or Qt).
* Better search (by name, father’s name, etc.).

