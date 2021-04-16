# Installing Red Hat CodeReady Containers on Windows 10 Pro

Note: Windows 10 Pro is required to run CodeReady Containers as Hyper-v support is required

- Enable Hyper-v on Windows 10 Pro. 1. In the search field next to the Windows icon, type 'Turn Windows Features onr or off' and click the Turn Windows Features onr or off (control panel) option in the popup dialog box. 2. In the Windows Features dialog, click the check box next to the Hyper-V option to enable Hyper-V.  3. Restart windows after Hyper-V has been enabled.

Follow the instructions [Create an OpenShift cluster](https://cloud.redhat.com/openshift/create/local) to install CodeReady Containers (CRC). Chose the "local" tab and select your OS.

- When you click the **Create an Openshift cluster** link, you will be redirected to login with your Red Hat customer portal user ID and password.  If you don't have one, click this link [Create one now](https://sso.redhat.com/auth/realms/redhat-external/login-actions/registration?client_id=cloud-services&tab_id=Y7oLs1FmAqY) to create a Red Hat customer portal user ID and password.

- On the **Create an Openshift cluster** go to step 1. **What you need to get started**.  In the **CodeReady Containers archive** section chose your OS (Windows) and click the **Download CodeReady Containers** button to start the download.

- In step 1. of the **Create an Openshift cluster** page also click the **Download Pull Secret** button to download the secret needed to start your CodeReady Containers instance.  I placed the pull-secret.txt file in a directory I created: C:\ Users\<Home Dir>\Documents\crc 

- To install crc, I created a directory called C:\Program Files (x86)\crc, copied the crc.exe file from the Downloads directory, and add this directory to the PATH statement.

- Run the crc setup command.  During the setup you chose to send or not send telemetry data to Red Hat. The crc setup command will enable Hyper-V if it is not already installed and enabled.  If Hyper-v is being setup for the first time, you will need to reboot your system.

      >crc setup
      
- To startup up CoderReady Containers use the crc startup command and include the path to the pull secret.

      >crc start -p "C:\Users\<Home Dir>\Documents\crc\pull-secret.txt"



