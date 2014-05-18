## **Install the {{include.pack}} package**

After updating the package list to ensure the latest version can be found, install the package(s) using the debian package installer.

    sudo apt-get update
    sudo apt-get --force-yes -y install {{include.pack}}
    
The "--force-yes -y" just confirms the package should be installed despite being from an un-official source.

*note - add any {% include link/int/pack-list %} to be installed at the same time to the command above*
