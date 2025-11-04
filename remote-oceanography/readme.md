
# A) Use Google Colab (no install needed)

1. **Create a Google account**

   * Go to Google and choose *Create account* → follow the prompts (name, email, password).

2. **Open Colab**

   * Visit Google Colab and sign in with your Google account.

3. **Create your first notebook**

   * Click **File → New notebook**.
   * Rename it (top-left), then run a test:

     ```python
     import sys, numpy as np
     np.mean([1,2,3]), sys.version
     ```

4. **Save and manage files**

   * Your notebook saves to **Google Drive** automatically.
   * To access Drive files in Colab:

     ```python
     from google.colab import drive
     drive.mount('/content/drive')
     ```
   * Upload local files with the left sidebar (Files) → **Upload**.

# B) Install Jupyter Notebook on your computer

You have two easy paths. If you’re new, **Anaconda** is simplest. If you already have Python, **pip** works fine.

## Option 1 — Anaconda (recommended, all-in-one)

1. **Install Anaconda**

   * Download the Anaconda installer for your OS (Windows/macOS/Linux) and run it.
   * During install, allow it to add Anaconda to your PATH (or use the Anaconda Prompt on Windows).

2. **Launch Jupyter Notebook**

   * **Windows:** Open **Anaconda Prompt**, run:

     ```bat
     jupyter notebook
     ```
   * **macOS/Linux:** Open **Terminal**, run:

     ```bash
     jupyter notebook
     ```
   * Your browser opens at `http://localhost:8888`. Click **New → Python 3** to create a notebook.

## Option 2 — Pip + virtual environment (lightweight)

> Works on Windows, macOS, and Linux.

1. **Install Python 3.10+** (from python.org) if you don’t have it.

2. **Create a project folder and a virtual environment**

   * **Windows (PowerShell):**

     ```powershell
     mkdir ocean-project; cd ocean-project
     python -m venv .venv
     .\.venv\Scripts\Activate.ps1
     ```
   * **macOS/Linux (Terminal):**

     ```bash
     mkdir ocean-project && cd ocean-project
     python3 -m venv .venv
     source .venv/bin/activate
     ```

3. **Install Jupyter Notebook (and common packages)**

   ```bash
   python -m pip install --upgrade pip
   python -m pip install notebook jupyterlab numpy pandas matplotlib xarray cartopy pywavelets
   ```

4. **Run Jupyter**

   ```bash
   jupyter notebook
   ```

   * Browser opens → **New → Python 3 (ipykernel)**.

# C) Verify everything works

In a new notebook cell, run:

```python
import numpy as np, pandas as pd, matplotlib.pyplot as plt
import xarray as xr
import sys
print("Python:", sys.version)
print("NumPy:", np.__version__)
print("Pandas:", pd.__version__)
plt.plot([0,1,2],[0,1,0]); plt.title("Test plot");
```

You should see version info and a simple plot.

# D) Useful tips (common issues)

* **“Command not found: jupyter”**
  Activate your environment (see step B-2) or reopen Terminal/Anaconda Prompt.
* **Pip cache/permission warning on Linux**
  Use:

  ```bash
  python -m pip install --user notebook
  ```

  or install inside a virtual environment (recommended).
* **Firewall pop-up**
  Allow local access so your browser can connect to `localhost:8888`.
* **Prefer JupyterLab**
  It’s a modern interface. Launch with:

  ```bash
  jupyter lab
  ```

If you tell me your OS (Windows/macOS/Linux), I can tailor the exact commands and a minimal “oceanography starter” environment (e.g., xarray + netCDF4 + cartopy setup) for you.
