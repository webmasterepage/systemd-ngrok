# Installation

Step 1: Place [`ngrok`](https://ngrok.com/download) in `/opt/ngrok/`.

Step 2: Get `authtoken` from ngrok website, then add it to `/opt/ngrok/ngrok.yml`.

Step 3. Modify your own configrations in `/opt/ngrok/ngrok.yml`.

Step 4: Add `ngrok.service` to `/lib/systemd/system/`.

Step 5: Start ngrok service by typing:

```
    systemctl enable ngrok.service
    systemctl start ngrok.service
```

or just execute `install.sh` on Linux x64 platform.

```
    curl -O https://raw.githubusercontent.com/vincenthsu/systemd-ngrok/master/install.sh
    chmod +x install.sh
    sudo ./install.sh <your_authtoken>
```
Install on background

sudo /opt/ngrok/ngrok start --all --config /opt/ngrok/ngrok.yml &
