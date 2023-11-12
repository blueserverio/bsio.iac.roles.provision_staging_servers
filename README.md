# BSIO IaC Role - Provision Staging Servers

## Overview
This Ansible role focuses on provisioning initial or "staging" servers essential for the environment's foundational services. These servers, like HashiCorp Vault, NetBox, and MAAS, play an interim role before the more robust infrastructure is in place.

##### **Note**:

This repository is a subset of the larger BlueServer.io Infrastructure as Code project. For a comprehensive understanding and to get started with the overarching project, please refer to the [main project README](https://github.com/blueserverio/bsio.iac.provision_environment/blob/main/README.md).

## Role Variables

```yaml
---

```

## Dependencies

No Dependencies

## Example Playbook

```yaml
--- 
- name: Build Staging Servers
  hosts: workstation
  gather_facts: no
  tasks:
    - name: Build Staging Servers
      include_role: 
        name: bsio.iac.roles.provision_staging_servers
        tasks_from: provision_staging_servers
```

## Contributing
Your contributions are always welcome! If you're looking to contribute to our project, please first read our [CONTRIBUTING guidelines](https://github.com/blueserverio/bsio.iac.provision_environment/blob/main/CONTRIBUTING.md). We look forward to working together to improve and expand the project.


## License
This project is licensed under the [MIT License](LICENSE).
