# Installing Red Hat CodeReady Containers on Windows 10

Follow the instructions [Create an OpenShift cluster](https://cloud.redhat.com/openshift/create/local) to install CodeReady Containers (CRC). Chose the "local" tab and select your OS.

- When you click the **Create an Openshift cluster** link, you will be redirected to login with your Red Hat customer portal user ID and password.  If you don't have one, click this link [Create one now](https://sso.redhat.com/auth/realms/redhat-external/login-actions/registration?client_id=cloud-services&tab_id=Y7oLs1FmAqY) to create a Red Hat customer portal user ID and password.

- On the **Create an Openshift cluster** go to step 1. **What you need to get started**.  In the **CodeReady Containers archive** section chose your OS (Windows) and click the **Download CodeReady Containers** button to start the download.

- In step 1. also click the **Download Pull Secret** button to download the secret needed to start your CodeReady Containers instance.  I placed the pull-secret.txt file in the C:\ Users\<Home Dir>\Documents\crc directory

- To install crc, I created a directory called C:\Program Files (x86)\crc, copied the crc.exe file from the Downloads directory, and added the directory to the PATH statement.

- Run the crc setup command.  During the setup you chose to send or not send telemetry data to Red Hat.

      >crc setup


