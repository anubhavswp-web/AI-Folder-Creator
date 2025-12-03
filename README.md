# 📁 AI-Powered Folder Structure Generator  
### *Prompt-Engineered Automation for STEM Content Development*

---

## 🚀 Overview  
This project is an **AI-assisted automation tool** that reads an Excel/CSV file containing *main topics* and *subtopics* (e.g., AP Calculus or STEM study units) and automatically generates a complete, hierarchical folder structure on the user's computer.

It was developed using a combination of:

- **Prompt Engineering**
- **Python Automation**
- **Iterative AI-based reasoning**
- **Structured data parsing**
- **User-centric workflow design**

This tool eliminates hours of manual work for educators, curriculum designers, and STEM content creators.

---

## 📂 Example Input File Format  
**Row 1:** Header (ignored)  
**Column A:** Main Topics  
**Column B:** Subtopics  

A2: 1. The Chain Rule | B2: 1.1 Composition of Functions Review
A3: (empty) | B3: 1.2 Understanding the Need for Chain Rule
A4: (Main topic 2) | B4: 2.1 First subtopic of main topic 2

---

## 🛠️ How to Run the Script  

### **Using PowerShell**
```powershell
python "D:\New project\Sub folder creater\create_drive_folders_local.py"
What Happens Next:

A file-picker window opens → choose your .xlsx or .csv

You enter your root path (or press Enter to accept default)

The folder system is generated automatically

📘 Technologies Used

Python 3.x

Pandas

Tkinter (GUI file picker)

OS & Pathlib

Prompt Engineering / LLM-assisted development

👤 About the Author

Anubhav Swaroop
Prompt Engineer | AI Automation Specialist | STEM Content Generator

I build tools that accelerate STEM education, automate repetitive workflows, and enable educators to scale their output.

---

## 💡 Why This Project Exists  
As a STEM content generator, I often work with complex outlines containing:

- Dozens of **main topics**  
- Hundreds of **subtopics**  
- Hierarchical study material  
- Multiple course units  

Manually creating folder structures for each unit was:

- ❌ Time-consuming  
- ❌ Error-prone  
- ❌ Zero creativity value  

So I built this automation with AI guidance — transforming complex topic spreadsheets into clean folder systems.

---

## 🔧 What This Tool Does  
Given an Excel or CSV file, the tool:

### ✔ Reads only the **first two columns**  
- Column A → Main Topics  
- Column B → Subtopics  

### ✔ Creates a **parent folder** named after the file  
Example:  
`AP_Calculus_BC_Unit3_Differentiation_Composite_Implicit_Inverse`  

### ✔ Builds subfolders according to strict logic:
- For each main topic:
  - Creates a folder  
  - Collects subtopics:
    - Subtopic can be on the **same row** as the main topic  
    - Subtopics can appear up to **5 rows apart**  
    - Looks forward up to **50 rows** for the next main topic  
- Stops subtopic collection when:
  - Next main topic appears  
  - >5 blank rows in Column B  
  - End of file  

### ✔ Automatically sanitizes folder names
- Removes emojis and invalid symbols  
- Replaces `:` with ` -`  
- Handles Windows forbidden filenames  
- Eliminates trailing dots/spaces  

### ✔ Uses a GUI file picker for easy use  
(You don’t need to type file paths manually.)

---

## 🧠 Prompt Engineering Contribution  
This project is more than Python coding — it is a **prompt engineering case study**.

Key skills demonstrated:

### ### 🔹 Translating ambiguous human logic into deterministic behavior  
Example rules I created and refined using prompts:

- “Main topics appear within 50 rows”  
- “Subtopics appear within 5-row gaps”  
- “The first subtopic may appear on the same row as the main topic”  

### 🔹 Iterative debugging through natural-language reasoning  
The logic for:
- Skipping blank rows  
- Detecting next main topic  
- Preventing false positives  
- Handling inconsistent Excel structures  
was developed collaboratively with an LLM.

### 🔹 Full workflow design  
From conceptual prompt → algorithm → Python implementation → user-friendly execution.

This demonstrates real-world **PromptOps** and **AI-augmented engineering**.

---

<img width="1350" height="716" alt="Screenshot 2025-12-03 213557" src="https://github.com/user-attachments/assets/cac153ef-c8ab-4b0e-b06c-3206cd8d4a70" />
<img width="1355" height="702" alt="Screenshot 2025-12-03 213628" src="https://github.com/user-attachments/assets/e75df403-5d99-4fc4-b974-21c9a2827588" />




