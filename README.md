# Study_tracker
Track your study hours the smart way — a Java console app for logging study sessions, viewing summaries, and exporting reports to CSV.

---

This project demonstrates the use of **OOP concepts**, **Collections Framework**, **File Handling**, and **Date-Time API** in Java.

---

## 🚀 Features

* 📥 Add new study logs with subject, duration, and description
* 📄 View all stored study logs
* 📊 Generate study summary by **date**
* 📚 Generate study summary by **subject**
* 📁 Export study logs to a **CSV file**
* 🖥️ Simple menu-driven console interface

---

## 🛠️ Technologies Used

* **Java (JDK 8 or above)**
* `java.util` (ArrayList, TreeMap, Scanner)
* `java.time.LocalDate`
* `java.io.FileWriter`

---

## 🧩 Class Description

### 1️⃣ StudyLog

Represents a single study record.

* Attributes: Date, Subject, Duration, Description
* Includes getters and `toString()` method

### 2️⃣ StudyTracker

Handles core functionality:

* Insert new study logs
* Display all logs
* Summary by date
* Summary by subject
* Export logs to CSV

### 3️⃣ StudyTrackerMain

* Entry point of the application
* Displays menu and handles user input

---

## ▶️ How to Run the Application

1. Open terminal / command prompt
2. Compile the program:

   ```bash
   javac StudyTrackerMain.java
   ```
3. Run the application:

   ```bash
   java StudyTrackerMain
   ```

---

## 📑 Sample Menu

```
1 : Insert new study log into Database
2 : View all study logs
3 : Summary of study log by date
4 : Summary of study log by subject
5 : Export study log to CSV file
6 : Exit the application
```

---

## 📤 CSV Export Format

The exported file `MangeshStudy.csv` contains:

```
Date,Subject,Duration,Description
2026-01-11,Java,2.5,OOP concepts practice
```

---

## 🎯 Learning Outcomes

* Hands-on practice with Java OOP
* Use of ArrayList and TreeMap
* File handling using FileWriter
* Working with LocalDate
* Building menu-driven applications

---

## 👨‍💻 Author

**Mangesh Ashok Bedre**
