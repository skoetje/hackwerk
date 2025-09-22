# Code-Along: Company Explorer (Codam Test)

This notebook (`codam_test.ipynb`) builds an interactive app to explore Dutch company data.  
You’ll load a CSV, clean it, visualize on a map with Folium, and wrap it into a simple Gradio interface.

---

## 1. Prerequisites

- **Python 3.10+**  
- A terminal (Linux/macOS default, Windows PowerShell or CMD)  
- (Optional) Git if you clone this project  
- (Optional) VS Code or JupyterLab  

---

## 2. Install Python

### macOS
```bash
brew install python@3.11
python3 --version
```

### Linux (Ubuntu/Debian)
```bash
sudo apt update
sudo apt install -y python3.11 python3.11-venv python3-pip
python3 --version
```

### Windows
1. Install from the Microsoft Store or python.org (tick **Add Python to PATH**).
2. Confirm:
   ```powershell
   python --version
   ```
   or  
   ```powershell
   py --version
   ```

---

## 3. Quickstart Setup

1. Clone/download this repo and open a terminal in the folder.  
2. Create & activate a virtual environment:  

**Linux/macOS:**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

**Windows (PowerShell):**
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

3. Install dependencies:
```bash
pip install --upgrade pip
pip install jupyterlab gradio folium pandas
```

4. Place your CSV in the project root (default expected name: **`kvk_data_codam.csv`**).

---

## 4. Run the Notebook

```bash
jupyter lab
```

Open **`codam_test.ipynb`** and run cells from top to bottom.  

You’ll:  
- Clean and normalize company data  
- View interactive maps of locations  
- Explore attributes (active status, business descriptions, etc.)

---

## 5. Running as a Gradio App

Some cells create a **Gradio interface** for searching and exploring companies.  
If you want to run the app standalone:

1. Copy the Gradio code from the notebook into a new file, e.g. `app.py`:
   ```python
   import gradio as gr
   # (paste your search/map functions here)
   demo = gr.Interface(...)
   demo.launch()
   ```

2. Run:
   ```bash
   python app.py
   ```
   This starts a local web server at [http://localhost:7860](http://localhost:7860).

---

## 6. Suggested Project Layout

```
.
├─ codam_test.ipynb
├─ kvk_data_codam.csv       # your input dataset
├─ app.py                   # optional Gradio app
├─ requirements.txt
└─ README.md
```

**requirements.txt**:
```
gradio
folium
pandas
jupyterlab
```

Install with:
```bash
pip install -r requirements.txt
```

---

## 7. Common Issues

- **File not found:** Ensure `kvk_data_codam.csv` is in the repo folder.  
- **Maps not showing:** Run all cells, especially those with `folium.Map`.  
- **PowerShell script blocked (Windows):**  
  ```powershell
  Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
  ```
  Then re-activate `.venv`.

---

## 8. How to Code Along

1. Everyone sets up their environment.  
2. Open `codam_test.ipynb`.  
3. Run cleaning + exploration steps together.  
4. Explore map + search features.  
5. (Optional) Turn your notebook logic into a Gradio web app.  

---

🚀 You’re ready to code along and explore Dutch company data interactively!  
