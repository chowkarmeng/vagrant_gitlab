# vagrant_gitlab
This git repository will demonstrate how GitLab are installed as a stand-alone dockerized GitLab Community Edition server in a Ubuntu Focal VM orchestrated using Vagrant.

Vagrant will be used to create VM in Oracle VirtualBox. This intended to show case orchestration of Oracle VirtualBox using Hashicorp Vagrant, and making GitLab example as a turn-key sample without needing to installed files or services in your local machine.

The [GitLab Docker images | GitLab](https://docs.gitlab.com/ee/install/docker.html) may pose as a challenge for users to modify it to work on Windows based OS Hosts.

# Pre-requisites:
Internet connection
Windows OS Host with 16GB RAM or higher
> **Note:** The **VM** to run GitLab CE without memory trashing will need at least 8GB 

This Demo was tested on the following software installed in Windows 10
|                |Oracle VirtualBox Version|Hashicorp Vagrant Version                         |
|----------------|-------------------------------|-----------------------------|
|Older Configuration|[6.1.18 r142142](https://download.virtualbox.org/virtualbox/6.1.18/VirtualBox-6.1.18-142142-Win.exe)           |[2.2.15 i686](https://releases.hashicorp.com/vagrant/2.2.15/vagrant_2.2.15_i686.msi)            |
|Tested Configuration 1|[7.0.10 r158379](https://download.virtualbox.org/virtualbox/7.0.10/VirtualBox-7.0.10-158379-Win.exe)            |[2.3.7 i686](https://releases.hashicorp.com/vagrant/2.3.7/vagrant_2.3.7_windows_i686.msi)            |
|Tested Configuration 2 |[7.0.12 r159484](https://download.virtualbox.org/virtualbox/7.0.12/VirtualBox-7.0.12-159484-Win.exe)|[2.4.0 i686](https://releases.hashicorp.com/vagrant/2.4.0/vagrant_2.4.0_windows_i686.msi)|


# Steps

 1. Make sure Vagrant and VirtualBox is installed.
 2. git clone this repo.
 3. [Update your windows host  file](https://www.howtogeek.com/784196/how-to-edit-the-hosts-file-on-windows-10-or-11/) to have the gitlab.example.com to be pointed to 127.0.0.1
 4. Open the command prompt (Administrator mode is not needed).
 5. change directory into the cloned git repo 'localdev'
 6. Lastly, run "vagrant up"

> **Note:**  **DO NOT** use this example in a production environment as it is not **Hardened** with security best practices. 

