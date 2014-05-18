## **Add the repository**

To be able to locate and download a package the repository's address must be added to the sources list.

    sudo sh -c "echo 'deb http://archive.emonhub.org {{ include.dist }} unstable' >> /etc/apt/sources.list"
    
This only needs to be done once and then all the packages for the OpenEnergyMonitor project are accesible.
    
*note: If running a different {% include link/int/dist-list %} edit "{{ include.dist }}" to suit.*

