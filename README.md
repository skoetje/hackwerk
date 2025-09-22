A quick, friendly guide to get everyone set up—on Linux, macOS, or Windows—and ready to code along with the notebook in this repo.

✅ This project centers around a Jupyter notebook (codam_hackathon.ipynb). It reads a large JSON, explores/visualizes data, and includes bits that can be run in a Streamlit context.
🧰 Main libraries used: pandas, numpy, ijson, plotly, pydeck, geopy, streamlit, streamlit-jupyter.

⸻

1) Prerequisites
	•	Python 3.11+
	•	A terminal (macOS/Linux default, Windows PowerShell or CMD)
	•	(Optional) Git if you plan to clone a repository
	•	(Optional) VS Code or your favorite editor

If you already have Python 3.11+ and pip, you can skip to Quickstart.

2) Install Python 3.11+

macOS
	•	Easiest via Homebrew:
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install python@3.11

python3 --version

sudo apt update
sudo apt install -y python3.11 python3.11-venv python3-pip
python3 --version

Windows (PowerShell)
	1.	Install from the Microsoft Store or download from python.org (choose Add Python to PATH during setup).
	2.	Confirm:

 py --version

 3) Quickstart (in 90 seconds)
	1.	Clone or download this project and open a terminal in the project folder.
	2.	Create & activate a virtual environment

macOS / Linux (bash/zsh)
python3 -m venv .venv
source .venv/bin/activate

Windows (PowerShell)
python -m venv .venv
.\.venv\Scripts\Activate.ps1

	3.	Install dependencies
 pip install --upgrade pip
pip install jupyterlab pandas numpy ijson plotly pydeck geopy streamlit streamlit-jupyter

	4.	Launch Jupyter to run the notebook
 jupyter lab

 Then open codam_hackathon.ipynb and run cells top-to-bottom.
