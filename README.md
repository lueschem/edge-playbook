# edge-playbook

Ansible playbook that configures selected features on an edge device.

## Features

### Monitoring

Feature activation:

- monitoring_enabled: true

Required parameters for monitoring:

- monitoring_influxdb_server: INFLUXDB_SERVER
- monitoring_influxdb_bucket: INFLUXDB_BUCKET
- monitoring_influxdb_http_token: INFLUXDB_SECRET_TOKEN
- monitoring_influxdb_org: INFLUXDB_ORGANIZATION

### Kiosk Screen

Feature activation:

- kiosk_enabled: true

Required parameters for kiosk screen:

- kiosk_kiosk_url: https://some.page.com

### Github Actions Runner

Feature activation:

- gharunner_enabled: true

Required parameters for repository runner:

- gharunner_github_account: GH_USER
- gharunner_github_repo: GH_REPO
- gharunner_access_token: GH_SECRET_TOKEN

Optional parameter if the runner shall be re-installed during an OS update:

- gharunner_reinstall_runner: yes (default yes)
