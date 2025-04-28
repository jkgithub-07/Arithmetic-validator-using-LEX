# Arithmetic-validator-using-LEX


**Arithmetic Expression Validator** is designed to **validate arithmetic expressions** via a **web interface** using **Flask** and **LEX**
This tool checks whether a given arithmetic expression is **valid** using a **Lexical Analyzer** running behind a Python Flask server.

---

## 📚 Project Overview

This project connects a simple **frontend web form** to a **Flask backend**, which then **executes a LEX program** to validate user-submitted arithmetic expressions.  
The system checks for correct usage of:
- Operators (`+`, `-`, `*`, `/`)
- Numbers (operands)
- Balanced parentheses `(` and `)`
- Syntax correctness

---

## ✨ Features

- 🌐 Web interface for user input
- 🛡️ Server-side validation using a compiled LEX program
- 📜 Lightweight, fast, and easy to use
- 🔥 Full-stack architecture (Frontend + Backend + LEX integration)
- 🧩 Easy to expand for more complex grammar rules

---

## 🛠️ Technologies Used

- **Frontend:** HTML/CSS (basic form)
- **Backend:** Python Flask
- **Validation:** LEX (Flex) + C
- **Server:** Localhost (Flask Development Server)

---

## 🚀 Installation and Setup

### 1. Prerequisites
- Python 3.12.7
- Flask (`pip install flask`)
- LEX/Flex and GCC compiler

### 2. Clone the repository
```bash
git clone https://github.com/jkgithub-07/arithmetic-validator-using-LEX.git
cd arithmetic-validator-using-LEX
```

### 3. Compile the LEX Program
```bash
flex validator.l
gcc lex.yy.c -o validator -lfl
```

This will generate an executable file named `validator`.

### 4. Set up the Flask App
Install the required Python packages:
```bash
pip install -r requirements.txt
```


### 5. Run the Flask Server
```bash
python app.py
```

By default, the app will run at:  
➡️ `http://127.0.0.1:5000/`

---

## 🌟 Usage

1. Open your browser and navigate to `http://127.0.0.1:5000/`
2. Enter an arithmetic expression (e.g., `(3 + 4) * 5`)
3. Submit the form
4. The server will:
   - Pass the expression to the LEX validator
   - Receive the validation result (Valid / Invalid)
   - Display the result on the page ✅❌

---

## 🧩 Project Structure

```bash
.
├── app.py              # Flask server
├── validator.l         # LEX code for validation
├── templates/
│   └── index.html      # Frontend HTML form
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```








