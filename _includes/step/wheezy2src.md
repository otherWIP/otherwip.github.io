#### **Add the repository url and update the sources list.**

    sudo sh -c "echo 'deb http://archive.emonhub.org {{ include.dist }} unstable' >> /etc/apt/sources.list"
    
*note: If running a different {% include link/int/dist-list %} edit "{{ include.dist }}" to suit.*

