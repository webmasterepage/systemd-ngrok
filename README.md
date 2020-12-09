# Installation

just follow this on linux command.

```
    curl -O https://raw.githubusercontent.com/webmasterepage/systemd-ngrok/master/install.sh
    chmod +x install.sh
    sudo ./install.sh <your_authtoken>
    systemctl daemon-reload
``` systemctl enable ngrok.service
    systemctl start ngrok.service
    systemctl status ngrok.service
    
Install on background

sudo /opt/ngrok/ngrok start --all --config /opt/ngrok/ngrok.yml &
