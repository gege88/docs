---
title: Upgrade NetQ Agents on Cumulus Linux Switches
author: Cumulus Networks
weight: 143
toc: 5
---
The following instructions are applicable to both Cumulus Linux 3.x and 4.x, and for both on-premises and cloud deployments.

To upgrade the NetQ Agent:

1. Log in to your switch or host.

2. Update and install the new NetQ debian package.

    <details><summary>For Switches and Hosts Running Cumulus Linux or Ubuntu</summary>

    ```
    sudo apt-get update
    sudo apt-get install -y netq-agent
    ```

    </details>
    <details><summary>For Hosts Running RHEL or CentOS</summary>

    ```
    sudo yum update
    sudo yum install netq-agent
    ```

    </details>

4. Restart the NetQ Agent.

```
 netq config restart agent
```

Refer to {{<link title="Install and Configure the NetQ Agent on Cumulus Linux Switches">}} to complete the upgrade.
