# Quick Start

Welcome! This guide will help you get started with the NMFS Openscapes JupyterHub.

## Prerequisites

Before you begin, make sure you have:

1. **GitHub Account**: You'll need a GitHub account to log in. Create one at <https://github.com/signup> if you don't have one.
2. **Web Browser**: We recommend using Chrome, Firefox, or Safari. Make sure your browser is up to date.

## Getting Started

### Step 1: Log In

1. Go to <https://nmfs-openscapes.2i2c.cloud/>
2. Click **"Login to continue"**
3. Log in with your GitHub account if prompted
4. Authorize the JupyterHub application to access your GitHub account

### Step 2: Select Your Environment

After logging in, you'll be asked to choose:

1. **Image Type**: Select the environment that matches your needs
   - **Openscapes Python** (default): Python with geospatial packages
   - **Openscapes R**: R and RStudio with common packages
   - **Geospatial**: Python and R with geospatial libraries

2. **Server Size**: Choose based on your computational needs
   - **Small** (2 GB RAM): Sufficient for most tutorials and light analysis
   - **Medium** (8 GB RAM): For larger datasets
   - **Large** (16 GB RAM): For intensive computations (use sparingly)

3. Click **Start** and wait for your server to start (may take 1-2 minutes)

### Step 3: Explore the Interface

Once your server starts, you'll see the JupyterLab interface with a Launcher showing:

- **Notebook**: Create a new Jupyter notebook (Python, R, etc.)
- **Console**: Interactive Python or R console
- **Terminal**: Command-line access
- **RStudio**: Full RStudio IDE (opens in a new tab)
- **Other**: Text files, markdown files, and more

## Next Steps

Now that you're up and running:

1. **Learn JupyterLab basics**: See [Intro to JupyterLab](02-intro-to-lab.md)
2. **Learn RStudio basics**: See [RStudio](02-rstudio.md)
3. **Set up Git**: See [Git in JupyterLab](02-git-jupyter.md)
4. **Explore tutorials**: Browse the skills sections in the navigation

## Important Notes

- **Saving Work**: Your files are automatically saved in your home directory and persist between sessions
- **Logging Out**: Always log out when done (File → Log Out) to free up resources
- **Automatic Timeout**: Your session will automatically shut down after 90 minutes of inactivity
- **Lost Session**: If your server crashes, go to File → Hub Control Panel → Stop My Server, then restart

## Getting Help

If you run into issues:

- Check the [FAQ](../topics-skills/01-intro-to-jupyterhub.md#faq)
- Post in [Discussions](https://github.com/nmfs-opensci/NOAAHackDays/discussions)
- Report bugs in [Issues](https://github.com/nmfs-opensci/NOAAHackDays/issues)

Happy computing!
