# edge-playbook

Ansible playbook that configures selected features on an edge device.

## Features

### Kiosk Screen

Feature activation:

- kiosk_enabled: true

Required variables for kiosk screen:

- kiosk_kiosk_url: https://some.page.com

### Github Actions Runner

Feature activation:

- gharunner_enabled: true

Required variables for repository runner:

- gharunner_github_account: MY_GH_USER
- gharunner_github_repo: MY_GH_REPO
- gharunner_access_token: MY_SECRET_TOKEN

Optional variable if the runner shall be re-installed during an OS update:

- gharunner_reinstall_runner: yes (default yes)
