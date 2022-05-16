laniakea.jupyterhub_express_config
=========

Ansible role to configure the express image of JupyterHub in Laniakea after its deployment.
The jupyterhub service is enabled and started and the jupyterhub admin password is changed.

Role Variables
--------------

| Variable       | Description                      | Default                |
| -------------- | -------------------------------- | ---------------------- |
| username       | JupyterHub admin username        | jupyterhub             |
| service        | Name of the JupyterHub unit file | jupyterhub.service     |
| port           | Port where JupyterHub is served  | 80                     |
| export_dir_tar | Path to the export dir archive   | /opt/export_dir.tar.gz |


Example Playbook
----------------

```yml
- hosts: all
  roles:
    - role: "laniakea.jupyterhub_express_config"
      become: true
```

License
-------


Author Information
------------------

[Daniele Colombo](https://github.com/dacolombo)