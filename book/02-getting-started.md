# Getting Started

Welcome! This guide will help you get started with the JupyterHub.

## Prerequisites

Before you begin, make sure you have:

1. **GitHub Account**: You'll need a GitHub account to log in. Create one at <https://github.com/signup> if you don't have one.
2. **Web Browser**: We recommend using Chrome, Firefox, or Safari. Make sure your browser is up to date.

## Step 1: Log in and authenticate

Go to {{jupyterhub_url}} and click **“Login to continue”**.

You will be asked to log in with your GitHub Account, if you are not logged in already.

![JupyterHub Login](./img/jhub.png)

### Authorize the JupyterHub application

The first time you log in, GitHub will ask you to authorize the JupyterHub application to access your GitHub account. Approve/authorize when prompted so the Hub can verify your login.

If you run into issues logging in, try:
- Confirm you are logged into the correct GitHub account in your browser
- Try logging out of GitHub and logging in again
- Try a private/incognito window

## Step 2: Select your environment (image) and server size

After logging in, you'll be asked to choose:

### Image type

Select your image type from the drop-down. The default is our a geospatial image with Python and R.  Other images are in the dropdown. 

You can also use any image that works with a JupyterHub or point to a GitHub repo with an `environment.yml` file, and an image will be built for you. See [Other images](topics-skills/04-other-images.md) for how to use the JupyterHub with images not listed in the dropdown.


### Virtual machine size

You'll see a dropdown that allows you to choose the size of virtual machine. For the tutorials, you will only need the smallest virtual machine. Please only choose the large machines if you run out of RAM as the larger machines cost us more.

![Machine Profiles](./img/servers.png)

## Step 3: Start your server

After selecting your image and server size, click **Start**. JupyterHub will allocate your virtual machine. This may take several minutes.

![Jupyterhub Spawning](./img/spawning.png)

## Step 4: Use the Launcher (JupyterLab) to open tools

When you are in the JupyterLab tab (note the Jupyter logo), you will see a Launcher page. If you don't see this, go to **File → New Launcher** or click the blue button on the top left.

From the Launcher, you will see buttons to open:
- A new Jupyter notebook
- **RStudio** (opens in a new browser tab)
- Desktop / VSCode (if enabled)
- A Terminal
- Text files and Markdown files

![Jupyterhub Launcher](./img/jhub-launcher.png)

Clicking on the "Python 3", Terminal, Text File and Markdown File buttons will open a new tab in JupyterLab. You can also use the File dropdown menu for these.

To get an overview of JupyterLab, go here: [Intro to JupyterLab](./topics-skills/02-jupyter-lab.md)

## Opening RStudio

If you click the **RStudio** button in Launcher, RStudio will open in a new browser tab.

![RStudio](./img/rstudio.png)

To get an overview of RStudio, go here: [Intro to RStudio](./topics-skills/02-rstudio.md)

## Your files and shared folders

When you start your server, you will have access to your own virtual drive space. No other users will be able to see or access your files. You can upload files to your virtual drive space and save files here. You can create folders to organize your files.

Your personal directory is `home/jovyan`. Everyone has the same home directory path, but your files are separate and cannot be seen by others.

### Shared files

In the file panel, you will see a folder called `shared`. These are read-only shared files that we have prepared for you.

You will also see `shared-public`. This is a read-write folder for you to put files for everyone to see and use. You can create a team folder here for shared data and files.

> Note: everyone can see and change files in `shared-public`, so communicate with your team so multiple people don’t work on the same file at the same time.

![Shared folder](./img/shared-folder.png)

## Ending your session (log out / stop server)

When you are finished working for the day you should log out of the JupyterHub, although it will log you out automatically after 90 minutes. You will not lose work; your home directory is persistent.

When you keep a session active it uses up cloud resources (costs money) because it keeps a series of virtual machines deployed.

> **You log out from the JupyterLab tab not the RStudio tab.**

**From the JupyterLab browser tab**, do one of two things to stop the server:

- Log out **File → Log Out** and click "Log Out"!
- or **File → Hub Control Panel → Stop My Server**

> **Can’t find the JupyterLab tab? Go to {{jupyterhub_url}}/hub/home**

Logging out or stopping your server will **NOT** cause any of your work to be lost or deleted. It simply shuts down resources (equivalent to turning off your computer at the end of the day).

## Restarting your server

Sometimes your server will crash/stop. If that happens, go to the JupyterLab tab and then:
**File → Hub Control Panel → Stop My Server**, and then **Start My Server**.

You shouldn't lose your work unless you were uploading a file at the time.

## Getting help

- Slack: 
- Issues (bugs / package requests): 


### Acknowledgements

Some sections of this document have been taken from hackweeks organized by the University of Washington eScience Institute, CryoCloud and Openscapes.
