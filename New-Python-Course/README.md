# Python Programming Course

A comprehensive, hands-on Python programming course covering 18 topics — from the fundamentals of programming all the way to real-world application development.

---

## How to Access the Course

### Step 1: Learn on Publica Academy

The primary learning experience takes place on the **Publica Academy** platform. Here you will find everything you need to complete the course:

- **Slides** — structured, topic-by-topic lesson content
- **Projects** — hands-on assignments to apply what you have learned
- **Micro-topic Practice** — bite-sized exercises on each concept, guided by **Publius**, our AI learning assistant
- **Assessment** — end-of-topic quizzes and evaluations to test your understanding

> Visit [Publica Academy](https://publica.ai) to get started.

---

### Step 2: Deepen Your Understanding Here (This Repository)

This GitHub repository is your companion resource for **refined understanding and hands-on coding practice**. For each of the 18 topics you will find:

| File | Purpose |
|------|---------|
| `topic_XX_codebook.ipynb` | Interactive Jupyter notebook with explanations, code examples, activities, and a cumulative project |
| `topic_XX_project.md` | Detailed project brief with instructions and mark breakdown |

---

## Course Topics

| # | Topic |
|---|-------|
| 01 | [Intro to Programming](Topic_01_Intro_to_Programming) |
| 02 | [Python Syntax Basics](Topic_02_Python_Syntax_Basics) |
| 03 | [Variables & Data Types](Topic_03_Variables_Data_Types) |
| 04 | [Operators & Expressions](Topic_04_Operators_Expressions) |
| 05 | [Control Flow: Conditionals](Topic_05_Control_Flow_Conditionals) |
| 06 | [Control Flow: Loops](Topic_06_Control_Flow_Loops) |
| 07 | [Strings](Topic_07_Strings) |
| 08 | [Lists & Tuples](Topic_08_Lists_Tuples) |
| 09 | [Sets & Dictionaries](Topic_09_Sets_Dictionaries) |
| 10 | [Functions](Topic_10_Functions) |
| 11 | [Error Handling](Topic_11_Error_Handling) |
| 12 | [Modules & Packages](Topic_12_Modules_Packages) |
| 13 | [File Handling](Topic_13_File_Handling) |
| 14 | [OOP Basics](Topic_14_OOP_Basics) |
| 15 | [OOP Core Concepts](Topic_15_OOP_Core_Concepts) |
| 16 | [External Libraries (NumPy, Pandas, Matplotlib)](Topic_16_External_Libraries) |
| 17 | [Algorithms & Problem Solving](Topic_17_Algorithms_Problem_Solving) |
| 18 | [Python for Real-World Tasks (Capstone)](Topic_18_Python_Real_World) |

---

## How to Use the Notebooks

You have two options for running the Jupyter notebooks — **Google Colab** (no setup required) or **VS Code** (local environment).

---

### Option A: Google Colab (Recommended for Beginners)

No installation needed. Runs entirely in your browser.

1. Open [Google Colab](https://colab.research.google.com)
2. Click **File → Open notebook**
3. Select the **GitHub** tab
4. Paste this repository URL: `https://github.com/Publica-AI/academy-courses-v3`
5. Browse to the topic folder and open the `.ipynb` file you want
6. Click **Runtime → Run all** to execute all cells, or run them one by one with `Shift + Enter`

> You will need a free Google account to use Colab.

---

### Option B: VS Code (Recommended for Full Setup)

#### 1. Install Python

- Download Python 3.10 or later from [python.org/downloads](https://www.python.org/downloads/)
- During installation, check **"Add Python to PATH"**
- Verify the installation by opening a terminal and running:
  ```bash
  python --version
  ```

#### 2. Install VS Code

- Download VS Code from [code.visualstudio.com](https://code.visualstudio.com)
- Install the following extensions from the Extensions panel (`Ctrl + Shift + X`):
  - **Python** (by Microsoft)
  - **Jupyter** (by Microsoft)

#### 3. Clone This Repository

```bash
git clone https://github.com/Publica-AI/academy-courses-v3.git
cd academy-courses-v3/New-Python-Course
```

#### 4. Install Required Libraries

```bash
pip install notebook numpy pandas matplotlib requests
```

#### 5. Open a Notebook

- Open the cloned folder in VS Code: **File → Open Folder**
- Navigate to any topic folder (e.g. `Topic_01_Intro_to_Programming`)
- Click the `.ipynb` file to open it
- Select your Python interpreter when prompted (top-right of the notebook)
- Run cells with `Shift + Enter`

---

## Setting Up Python (Quick Reference)

| Step | Windows | Mac / Linux |
|------|---------|-------------|
| Install Python | [python.org/downloads](https://www.python.org/downloads/) — check "Add to PATH" | `brew install python3` or [python.org/downloads](https://www.python.org/downloads/) |
| Verify install | `python --version` in Command Prompt | `python3 --version` in Terminal |
| Install packages | `pip install numpy pandas matplotlib` | `pip3 install numpy pandas matplotlib` |
| Launch Jupyter | `jupyter notebook` | `jupyter notebook` |

---

## Cloning the Repository

If you want a local copy of all notebooks on your computer:

```bash
# Clone the repository
git clone https://github.com/Publica-AI/academy-courses-v3.git

# Navigate into the course folder
cd academy-courses-v3/New-Python-Course

# Open in VS Code
code .
```

To keep your local copy up to date with any future changes:

```bash
git pull origin main
```

---

## Need Help?

- Use **Publius** on the Publica Academy platform for guided support
- Raise an issue in this repository if you find a bug or error in a notebook

Happy coding!
