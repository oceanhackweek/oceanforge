# Working in the JupyterHub

The JupyterHub supports multiple interfaces for working with data, code, and files.
The two primary interfaces are **JupyterLab** and **RStudio**, with the **terminal**
available in both.

All interfaces operate on the same underlying filesystem. You can switch between
them at any time without copying files.

---

## JupyterLab

JupyterLab is a flexible web-based environment for working with notebooks,
scripts, and data files. In a Jupyter notebook, the code is run in code blocks with the output (like plots) shown in the notebook.

![JupyterLab Interface](./img/jupyterlab.png)

JupyterLab is a common IDE for Python users, but in our JupyterHub, it also has an R kernel so you can work equally well in R in JupyterLab.

### Key features

- Notebook interface for Python and R
- File browser and text editor
- Launcher for new notebooks, terminals, and other tools
- Integrated Git extension

For a more detailed introduction, see:
[Intro to JupyterLab](./topics-skills/02-jupyter-lab.md)

---

## RStudio

RStudio is a common IDE for R users and is customized for the features like package installation, Quarto integration, notebook + console. RStudio also uses notebook (RMarkdown or Quarto) but the output is not part of a saved notebook and the notebook is plain ascii so is easier for version control.

![RStudio Interface](./img/rstudio.png)

RStudio opens in a **separate browser tab**, but it uses the home directory as JupyterLab.

### Key features

- Script editor and R console
- Start new projects or files with templates
- Quarto integration
- Plots, packages, and help panels
- Integrated Git support
- Familiar IDE layout for R users

For a more detailed introduction, see:
[Intro to RStudio](./topics-skills/02-rstudio.md)

---

## The terminal

The terminal provides direct access to the command line.

You can open a terminal:
- From the JupyterLab Launcher
- From within RStudio

![Terminal](./img/terminal.png)

Use the terminal to:
- Run shell commands
- Manage files
- Use Git
- Run R or Python from the command line

Many advanced workflows rely on the terminal regardless of whether you use
JupyterLab or RStudio. 

---

## Files and the shared filesystem

All interfaces share the same filesystem.

Your personal working directory is `\home\jovyan`.

Files created in:
- JupyterLab
- RStudio
- The terminal

are immediately visible in the others.

### Shared folders

You will see shared folders such as:

- `shared` – read-only files prepared by organizers
- `shared-public` – read/write space shared across users

![Shared folder](./img/shared-folder.png)

> Files in `shared-public` can be edited by anyone. Coordinate with your team
to avoid overwriting each other’s work.

---

## Switching between interfaces

You can freely switch between JupyterLab and RStudio during a session.

Typical workflows include:

- Wrangling cloud data in Python in JupyterHub, saving intermediate files, loading those in R in RStudio.
- Exploring data in RStudio, then visualizing results in a notebook
- Running Git commands in the terminal, then continuing work in JupyterLab
- Editing scripts in RStudio and rendering outputs in JupyterLab

There is **no need to export or sync files manually**.

---

## When things go wrong

If an interface becomes unresponsive:
- In JupyterLab, try Kernel > Restart kernel or Shutdown All kernels
- Use **File → Hub Control Panel → Stop My Server**
- Restart the server

Your files in `/home/jovyan` are persistent and should not be lost.

---

## Where to go next

- For version control workflows, see  
  [Version Control with Git](./04-version-control-with-git.md)
- For external data access and credentials, see  
  [Data Access and Credentials](./05-data-access-and-credentials.md)


