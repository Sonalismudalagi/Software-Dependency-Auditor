🧩 Software Dependency Auditor

🔍 Overview
Software Dependency Auditor is a web-based tool built using Python (Flask) that analyzes dependencies from a project's requirements.txt file. It helps developers maintain project health by identifying outdated, illegal, or restricted libraries and generating detailed reports for better dependency management.

🚀 Features
📁 Upload a requirements.txt file

🔎 Detect outdated libraries by comparing installed and latest versions from PyPI

🚫 Identify illegal or restricted libraries

📊 Generate and download detailed reports in JSON and CSV formats

⚡ Built using a simple and clean Flask web interface

🧠 Tech Stack
Layer	Technologies
Frontend	HTML, CSS
Backend	Python (Flask)
Libraries Used	requests, json, subprocess, os
Output Formats	JSON, CSV

🖥️ How It Works

Upload your requirements.txt file through the web interface.
The system scans the file and:
Compares installed versions with the latest PyPI versions.
Checks for illegal or restricted libraries.
Results are displayed neatly on the web page.
Users can download reports in JSON or CSV format.

⚙️ Installation & Setup

1️⃣ Clone the Repository
git clone https://github.com/<your-username>/Software-Dependency-Auditor.git
cd Software-Dependency-Auditor

2️⃣ Create a Virtual Environment
python -m venv venv
venv\Scripts\activate   # On Windows
# OR
source venv/bin/activate  # On macOS/Linux

3️⃣ Install Dependencies
pip install flask requests pandas matplotlib

4️⃣ Run the Application
python app.py


Then open your browser and go to:
👉 http://127.0.0.1:5000

🧾 Example Output (Sample JSON Report)
{
    "filename": "requirements.txt",
    "dependencies": [
        "flask==2.3.2",
        "requests==2.31.0",
        "numpy==1.26.0"
    ],
    "outdated_libs": [
        "flask: Installed (2.3.2), Latest (3.1.0)"
    ],
    "illegal_libs": [],
    "report_generated": true
}

📸 Screenshots

<p align="center">
  <img width="1920" height="1020" alt="Screenshot 2025-04-20 205106" src="https://github.com/user-attachments/assets/88446d9b-84e6-4452-96c8-29e4e36e14f4" />
  <br>
  <em>📊 Screenshot showing analyzed dependencies and report view.</em>
  
</p>

🧩 Future Enhancements

Integrate dependency tree visualization (D3.js)

Include security vulnerability scanning (CVE lookup)

Allow direct GitHub repository analysis

Add dark mode for UI

🧑‍💻 Author

Sonali Mudalagi
🎓 4th Year Computer Science Engineering Student
💡 Passionate about Python, AI, and Web Development
