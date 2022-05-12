Role Name
=========

Ansible role to configure the express image of JupyterHub in Laniakea after its deployment.
The jupyterhub service is enabled and started and the jupyterhub admin password is changed.

Role Variables
--------------

| Variable | Description                      | Default            |
| -------- | -------------------------------- | ------------------ |
| username | JupyterHub admin username        | jupyterhub         |
| service  | Name of the JupyterHub unit file | jupyterhub.service |
| port     | Port where JupyterHub is served  | 80                 |


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