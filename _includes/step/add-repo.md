## **Add the repository location**

For the Pi to be able to locate and download a package the repository address must be added to the sources list.

    sudo sh -c "echo 'deb http://archive.emonhub.org {{ include.dist }} unstable' >> /etc/apt/sources.list"
    
*note: If running a different {% include link/int/dist-list %} edit "{{ include.dist }}" to suit.*

