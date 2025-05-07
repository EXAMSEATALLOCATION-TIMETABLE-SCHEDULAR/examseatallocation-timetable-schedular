# examseatallocation-timetable-schedular
# Exam Seating Allocation System

A Java-based desktop application that streamlines the process of allocating students to examination rooms, scheduling exam timetables, and visualizing seating arrangements. Designed with Swing for an intuitive UI, the system prioritizes real-time control, scalability, and flexibility—eliminating the need for databases or arrays by leveraging LinkedLists and file handling.

## 📌 Features

- 📂 **Upload Multiple Student Files**: Supports `.txt` file uploads for different years and branches.
- 🪑 **Smart Room Allocation**:
  - Dynamic allocation based on seats per room.
  - Filter students by year, branch, and section.
  - Mix students from multiple branches with configurable limits.
  - Avoids duplication and maintains room capacity constraints.
- 📅 **Timetable Scheduler**:
  - Generates an exam timetable using DFS/Queue logic.
  - Allows holiday exclusion for flexible planning.
- 🖥️ **Modern Swing UI**:
  - Responsive UI with buttons for all core operations.
  - Allocation results shown using `JTable`.
  - Visual room layout rendering in a grid format.
- 🔁 **Undo/Reset Options**:
  - Supports clearing previous allocations and restarting without exiting.
- 💾 **Data Persistence**:
  - File-based data handling (no database required).
  - Reads from and writes to `.txt` files.

## 🛠️ Tech Stack

- **Language**: Java (no external libraries)
- **UI Framework**: Java Swing
- **Data Structures**: LinkedLists, Queues, Stacks
- **Storage**: File-based (`students.txt`, `subjects.txt`)

## 📁 Project Structure

ExamSeatingSystem/
│
├── SwingUI.java # Main UI file for user interaction
├── StudentInfo.java # Handles student details
├── SeatingLogic.java # Core logic for room allocation
├── Room.java # Room class for seat tracking
├── ExamScheduler.java # Handles timetable generation
├── students.txt # Input: student data (multiple allowed)
├── subjects.txt # Input: subject list with exam dates
└── README.md # Project documentation



## 🧪 Usage Instructions

1. Launch `SwingUI.java` from your Java IDE (e.g., VS Code, IntelliJ).
2. Use the **Upload Student Files** button to upload one or more `.txt` files.
3. Upload the `subjects.txt` file for exam scheduling.
4. Configure:
   - Seats per room
   - Branches to mix
5. Click **Allocate** to assign students to rooms.
6. Click **View Room Arrangement** to see allocations in a structured format.
7. Use **Visualize** for grid-based room layout view.
8. Use **Generate Timetable** to see the scheduled exams.

## 📝 File Format Guidelines

- **students.txt**
Section-A, John Doe, 23CS001
Section-B, Jane Smith, 23IT021

- **subjects.txt**
Data Structures, 2025-05-12
Operating Systems, 2025-05-15

## 🔒 Constraints

- No usage of arrays or HashMaps.
- LinkedLists are used for all collections.
- Dynamic Swing UI with 6 consistent buttons.
- Handles multi-branch and multi-year logic seamlessly.

## ✨ Future Enhancements

- Export seating plan as PDF
- QR-based hall ticket verification
- Auto-email exam schedules to students

## 📃 License

This project is open-source and free to use for academic and educational purposes.

---

