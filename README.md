## Prerequisites

- Linux operating system with installed `git`

## Installation

- set up

```bash

chmod +x dummy.sh
sudo cp dummy.sh /usr/bin/

# set up for the service
sudo cp dummy.service /etc/systemd/system/

# Now reload the systemctl
sudo systemctl daemon-reload
```

- Interacting with the dummy service

```bash
# Interacting with the service
sudo systemctl start dummy
sudo systemctl stop dummy
sudo systemctl enable dummy
sudo systemctl disable dummy
sudo systemctl status dummy

# Check the logs
sudo journalctl -u dummy -f