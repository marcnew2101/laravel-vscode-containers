## Creating a new Laravel project using dev containers in VSCode

### Windows:

> virtualization must first be enabled in the BIOS

Step 1 - Install Docker Desktop https://www.docker.com/products/docker-desktop


Step 2 - Install WSL https://docs.microsoft.com/en-us/windows/wsl/install
> powershell commands
* wsl --install
* wsl --set-default-version 2
* wsl --list --online
* wsl --install -d 'DistroName'
> (optional) linux distros can also be installed from the Microsoft Store

> use the following command to ensure the distro is running WSL v2:
* wsl -l -v


> (optional) use the following command to convert a WSL v1 distro to v2:
* wsl --set-version distro-name 2


Step 3 - Open Docker Desktop
* go to settings -> Resources -> WSL Integration
* enable all distros


Step 4 - Install Windows Terminal app https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=en-us&gl=US


Step 5 - Open Windows Terminal app
* from the drop-down, select the Linux distro you installed in step 2
> If you want to place the build inside the Windows file system, use cd.. until you reach the root Linux file system. Then cd into the mnt folder, and then cd into the c folder. You will now be in the "C" drive of the Windows file system. You can now cd further into whichever folder you want to place the build.


Step 6 - Paste this command into the terminal and run (install will take around 5 minutes):
> the 'sample_app' portion of the below command can be changed to any name you want for your app

'''
curl -s "https://laravel.build/sample_app?with=mysql,redis&devcontainer" | bash
'''


Step 7 - VSCode

Opening the project folder in VSCode will prompt you to install the Remote Containers plugin. After installation, VSCode will then recognize that the folder is a container and will prompt you to open it in a container.
> You may get a Windows system prompt to authorize firewall access for Docker Desktop

Once the container has finished running, open a web browser and type in "localhost". This should present you with the default (Laravel) home page.

From here, you can make slight changes to the /resources/views/welcome.blade.php file. Any changes made here should immediately take effect once you refresh your browser window.


### Resources
* YouTube tutorial - https://www.youtube.com/watch?v=ojWxCP1lT-Y
* Laravel - https://laravel.com/docs/9.x/installation