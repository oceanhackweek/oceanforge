# Checklist
## Required setup

### EarthData Login

If you do not already have an Earthdata login, then navigate to the Earthdata login [page](https://urs.earthdata.nasa.gov/),
register, and record username and password somewhere for use during the hackweek. 

### GitHub Account

If you do not already have a GitHub account, then navigate to [GitHub](https://github.com/), enter your email address and click on the green ‘Sign up for GitHub’ button. Keep  your username and password handy.

### JupyterHub

The JupyterHub is a pre-provisioned compute environment which can be accessed via a web browser. You will not need to install anything.
Please follow these instructions which will guide you through gaining access to the JupyterHub. 

1. [Watch this video](https://youtu.be/uZ2Uy376Az8) to get an orientation on our JupyterHub.

2. Sign in by navigating to the [JupyterHub](https://nmfs-openscapes.2i2c.cloud/). Instructions to sign in are in our Slack channel [here](https://fish-pace.slack.com/files/U09FQF586KU/F09FRKRN5PC/hub.md).

3. You will see server options. To start, you can stay with the default image and RAM. It can take several minutes for new servers to launch on the cloud. Once things are spun up, you will see your very own instance of a JupyterLab environment. 

![server_options](../img/server_options.png)

You will have access to your own virtual drive space under the `/home/jovyan` directory. No other users will be able to see or access your data files. You can add/remove/edit files in your virtual drive space. You will also have access to the  *`shared-public`* folder (read and write access). These are shared spaces so please make sure not to delete files from here unless they are yours.

4. *To save our community money, when you are finished working for the day it is helpful for you to explicitly stop your server before logging out of your JupyterHub session.* To shut your server down immediately when you’re exiting your session please select “File -> Hub Control Panel -> Stop my Server” then you can click the “Log Out” button. We ask this because when you keep a session active it uses up AWS resources and these resources cost money per hour of use. If you forget this step, though, the server will shut down automatically after 90 min of no use.
Logging out will **NOT** cause any files under your home directory to be deleted. It is equivalent to turning off your desktop computer at the end of the day.


