# masai-project-2
# 📚 Library Management System (Python + CSV)

A terminal-based library management system built in Python. It supports secure login, role-based access (Librarian and Member), and stores data in CSV files — simulating a mini database.

---

## 🚀 Features

### 👩‍🏫 Librarian:
- Register members
- Add new books
- Issue books to members
- Return books
- View overdue books

### 👤 Member:
- Search book catalogue
- View personal loan history

---

## 🔐 Authentication
- Role-based login system (`Librarian` and `Member`)
- Passwords stored securely using `bcrypt`
- Session-based access to features

---

## 🗃️ Data Storage (CSV Files)

| File | Description |
|------|-------------|
| `books.csv` | ISBN, Title, Author, TotalCopies, AvailableCopies |
| `members.csv` | MemberID, Name|Role, PasswordHash, Email, JoinDate |
| `loans.csv` | LoanID, MemberID, ISBN, IssueDate, DueDate, ReturnDate |

---

## 🧰 Tech Stack

- Python 3.x
- `bcrypt` for password hashing
- Standard libraries: `csv`, `datetime`, `os`

---

## 🏁 Getting Started

1. **Clone the repo**
```bash
git clone https://github.com/YOUR_USERNAME/library_system.git
cd library_system
pip install bcrypt
python main.py
library_system/
│
├── data/
│   ├── books.csv
│   ├── members.csv
│   └── loans.csv
│
├── main.py
├── auth.py
├── books.py
├── members.py
├── loans.py
├── utils.py
└── README.md
