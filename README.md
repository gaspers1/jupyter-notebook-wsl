### Using Jupyter Notebook in WSL (Windows Subsystem for Linux)



---

##### Prerequisites

- WSL must be enabled in Windows 10
- Virtualenv, Jupyter notebook must be installed via pip on system

---

##### Steps

Step in project folder and create virtual environment

```bash
virtualenv .venv
```

Activate virtual environment

```bash
source .venv/bin/activate
```

First time install kernel

```bash
pip install ipykernel
```

Set virtual environment in ipython kernel

```bash
ipython kernel install --user --name .venv
```

Run jupyter notebook

```bash
jupyter notebook --no-browser
```

Copy url to browser to run jupyter in localhost
