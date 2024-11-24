# Dummy System Service

Sample solution for the [dummy-system-service](https://roadmap.sh/projects/dummy-systemd-service) challenge from [roadmap](https://roadmap.sh)

## Prerequisites

- Linux operating system with installed `git`

## Installation

**Clone the Repository**

- Clone this repository into the local machine.

```bash
git clone --depth=1 https://github.com/Aj-Seven/DevOps-Projects.git
```

- set up

```bash

# set the script for execution
cd DevOps-Projects/dummy-systemd-service
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
```
