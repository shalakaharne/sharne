# Quick Start Guide for Installing and Configuring ownCloud

The open source software, ownCloud allows users to file sync and share data from any location and using any device any time. To use ownCloud, the server must be installed and configured by the administrator. Once installed and configured, administrators can and and enable users to connect to ownCloud.
This quick start guide briefs on how to perform the following:

  - Install ownCloud server
  - Install Desktop Client
  - Create User
  - Connect to ownCloud using Desktop Client

# Install ownCloud server
You must install and configure ownCloud server to let the users connect to and synchronize files and date to owncloud. An administrator can install and configure Owncloud server. To install ownCloud server, follow the steps given below:
1. Download the latest version of owncloud from owncloud download page.
2. Go to the *Tarball* section and right-click *Download Tar* and select *Copy Link Address*.
3. Log in to your server through SSH.
4. Go to the directory in which you want to install ownCloud.
5. Run the following command to download the Tar file (.tarbz2).
[server]$ wget <.tar.bz2 link copied in step2>
Example: 
[server]$ wget https://download.owncloud.org/community/owncloud-10.0.8.tar.bz2 
6.	Under Download Tar button in owncloud download page, right-click sha256 and select Copy link Address.
7.	Run the following command to download  *sha256*.
[server]$ wget <sha256 link copied in step 6>
Example: [server]$ wget https://download.owncloud.org/community/owncloud-10.0.8.tar.bz2.sha256 
8.	Run the following command to verify if the sha256 signature matches with .tar.bz2 file.
[server]$ sha256sum -c <sha256 signature> < <.tar.bz2 file>
Example: [server]$ sha256sum -c owncloud-10.0.8.tar.bz2.sha256 < owncloud-10.0.8.tar.bz2 
If the result is *OK*, decompress the .tar.bz2 file using the following command:
[server]$ tar xvjf <.tarbz2 file>
Example: [server]$ tar xvjf owncloud-10.0.8.tar.bz2
A new subdirectory called/owncloud in the same directory in which you executed the command.
9.	Open your browser and navigate to the /owncloud folder.
The common URL is example.com/owncloud
10.	Enter a username and password of your choice and click Finish setup.
For more information on downloading ownCloud, go to https://owncloud.org/download/#instructions-server.

# Install Desktop Cient
An administrator can install and configure Owncloud server. To install ownCloud Desktop Synchronization Client, follow the steps given below:
1.	Download the ownCloud latest version of ownCloud *Desktop Synchronization Client* from https://owncloud.com/download/#desktop-clients.
2.	Double-click the downloaded .msi file and click Run to run the installation.
3.	Follow the on-screen instructions to install owncloud client.
4.	Click *Finish* to complete installation.
The owncloud Desktop Synchronization Client is installed.
For more information on installing ownCloud and customizing oncloud for windows client, go to https://doc.owncloud.com/desktop/2.5/installing.html#

# Create a User
An administrator can add new user in the owncloud Web UI. Follow the steps given below to add a new user:
1.	Open ownCloud in your browser.
2.	Go to *User Management* page.
3.	In the *username* and *password* fields, enter the user name and password for the new user.
Note: The log in name can contain letters (a-z, A-Z), numbers (0-9), dashes (-), underscores (_), periods (.) and at signs (@).
4.	Click *create user*.
The user is created.
**Note:** To set owncloud to automatically send notification to the user with their new login information, you can select the Send email to new user check box in the control panel on the lower left navigation bar and enter the new user’s email address. 
For more information on managing users in ownCloud, refer https://doc.owncloud.org/server/9.0/admin_manual/configuration_user/ 


# Connect to ownCloud using Desktop client
As a user, you can connect to ownCloud Desktop client and synchronize your files and data. Follow the steps given below to connect to ownCloud server using your Desktop client.
1.	Open ownCloud desktop application. 
2.	Enter your server address in *Server Address* and click *Next*.
3.	Enter the username and password and click *Next*.
4.	Select *Sync everything from the server* to sync all the data in your account or *Choose what to sync* to select what you want to sync. 
5.	Click *Connect*.
The desktop client installation is complete and will be synchronized based on your selection.
