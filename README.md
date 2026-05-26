# 📚 Study Tracker

A command-line Java application to help students **log, track, and analyze** their study sessions — by subject, by date, and exportable to CSV.

---

## 🚀 Features

- ✅ **Add Study Logs** — Record subject, duration (in hours), and a description for each session
- 📋 **View All Logs** — Display the complete study history in a clean tabular format
- 📅 **Summary by Date** — See total hours studied on each date (sorted chronologically)
- 📖 **Summary by Subject** — See total hours invested per subject (sorted alphabetically)
- 📤 **Export to CSV** — Export your entire study log to `MarvellousStudy.csv` for use in Excel / Google Sheets

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | Java (JDK 8+) |
| Date Handling | `java.time.LocalDate` |
| Data Storage | `ArrayList` (in-memory) |
| Sorted Aggregation | `TreeMap` |
| File Export | `FileWriter` → CSV |

---

## 📁 Project Structure

```
StudyTracker/
│
├── StudyTrackerMain.java      # Entry point — main menu loop
├── StudyTracker.java          # Core logic (insert, display, export, summaries)
├── StudyLog.java              # Data model (Date, Subject, Duration, Description)
└── MarvellousStudy.csv        # Auto-generated on export (not committed)
```

> All three classes are currently in a single file. You can refactor them into separate `.java` files for better maintainability.

---

## ⚙️ Getting Started

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- A terminal / command prompt

### Compile

```bash
javac StudyTrackerMain.java
```

### Run

```bash
java StudyTrackerMain
```

---

## 🖥️ Usage

Once launched, you'll see an interactive menu:

```
Please select the appropriate option
1 : Insert new study log into Database
2 : View all study logs
3 : Summary of study log by date
4 : Summary of study log by subject
5 : Export study log to CSV file
6 : Exit the application
```

### Example — Adding a Log

```
Please provide the name of subject like C/C++/Java/OS/DS
> Java

Enter the time period of your study in hours
> 2.5

Please provide the description about the study for future reference
> Covered Collections framework and TreeMap usage
```

### Example — CSV Output (`MarvellousStudy.csv`)

```
Date,Subject,Duration,Description
2025-05-27,Java,2.5,Covered Collections framework and TreeMap usage
2025-05-27,OS,1.0,Process scheduling algorithms
```

---

## 📌 Known Limitations

- Data is **not persistent** — logs are lost when the application exits (no database/file loading on startup)
- Date is **auto-set to today** — no manual date entry supported yet
- Input validation is minimal — entering a non-numeric duration will throw an exception

---

## 🔭 Planned Improvements

- [ ] Load existing logs from CSV on startup (persistence)
- [ ] Allow manual date entry
- [ ] Filter/search logs by subject or date range
- [ ] Add input validation and error handling
- [ ] Migrate to a proper database (SQLite / MySQL)
- [ ] Build a GUI using JavaFX

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👨‍💻 Author

> *"Mangesh Ashok Bedre."*