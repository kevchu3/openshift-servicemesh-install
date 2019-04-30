OpenShift Service Mesh
======================

The following instructions for OpenShift Service Mesh were taken from the OpenShift documentation and are intended to facilitate an installation:
https://docs.openshift.com/container-platform/3.11/servicemesh-install/servicemesh-install.html

Requirements
------------

* OpenShift 3.11
* See supported configurations for more details:
  - https://docs.openshift.com/container-platform/3.11/servicemesh-install/servicemesh-install.html#supported-configurations

Setup
-----

Review `files/istio-installation.yaml` and update as necessary with parameters provided by the user, see documentation for configuration.

Deploy
------

Run the `install.yaml` Ansible playbook to deploy the Service Mesh resources:
```
ansible-playbook -i <inventory> install.yaml
```

Enable automatic sidecar injection with the `post-install.yaml` Ansible playbook:
```
ansible-playbook -i <inventory> post-install.yaml
```

Uninstall
---------

Run the `uninstall.yaml` Ansible playbook:
```
ansible-playbook -i <inventory> uninstall.yaml
```

License
-------

GPLv3

Author
------

Kevin Chung
