# ☕ Coffee Leaf Health Detector - Installation Guide

Welcome! This guide is designed for beginners. We'll walk you through setting up and running this tool step-by-step.

---

## 🛠️ Step 1: Pre-requisites (One-time Setup)

Before you start, you'll need to install two tools on your computer:

1.  **Python 3.9+**: The "engine" that runs the backend.
    *   Download it from [python.org/downloads](https://www.python.org/downloads/).
    *   **IMPORTANT**: During installation, make sure to check the box that says **"Add Python to PATH"**.
2.  **Git**: A tool for downloading ("cloning") code from GitHub.
    *   Download it from [git-scm.com](https://git-scm.com/).

---

## 📥 Step 2: Download the Code

Now, let's bring the code to your machine.

1.  Open your **Command Prompt** (on Windows) or **Terminal** (on Mac/Linux).
2.  Type the following command and press Enter:
    ```bash
    git clone https://github.com/sasankpanuganti/coffee_nutrition.git
    ```
3.  Go into the project folder:
    ```bash
    cd coffee_nutrition
    ```

---

## ⚙️ Step 3: Setup the Backend (The API)

The backend is where the "Brain" (Deep Learning model) lives.

1.  Navigate into the backend folder:
    ```bash
    cd backend
    ```
2.  **Create a Virtual Environment**: This keeps the project's tools separate from other things on your computer.
    ```bash
    python -m venv .venv
    ```
3.  **Activate it**:
    *   **Windows**: `.\.venv\Scripts\activate`
    *   **Mac/Linux**: `source .venv/bin/activate`
4.  **Install the "Brain's" requirements**:
    ```bash
    pip install -r requirements.txt
    ```
5.  **Run the Backend**:
    ```bash
    python app.py
    ```
    > You will see a message like `Running on http://127.0.0.1:5000`. **Do not close this window!**

---

## 🎨 Step 4: Setup the Frontend (The UI)

The frontend is the website you interact with.

1.  Open a **SECOND Command Prompt/Terminal** window.
2.  Go back into the project folder, then into the frontend's public folder:
    ```bash
    cd coffee_nutrition/frontend/public
    ```
3.  **Start a simple website server**:
    ```bash
    python -m http.server 3000
    ```
    > You will see a message like `Serving HTTP on 0.0.0.0 port 3000...`.

---

## 🚀 Step 5: Start Using It!

1.  Open your web browser (Chrome, Firefox, etc.).
2.  Type **`http://localhost:3000`** in the address bar and press Enter.
3.  You should now see the Coffee Leaf Health Detector! 🍃

---

## 💡 Troubleshooting for Beginners

*   **"python is not recognized"**: You forgot to check "Add Python to PATH" during installation. Re-install Python and make sure that box is checked.
*   **Permissions Error**: Try running your Command Prompt as "Administrator".
*   **Port 5000 or 3000 Busy**: If you see an error about a port being in use, close any other apps that might be running servers, or restart your computer.
