OpenShift Hostpath Examples
===========================

The following instructions for OpenShift Service Mesh were taken from the OpenShift documentation and are intended to facilitate an installation:
https://docs.openshift.com/container-platform/3.11/servicemesh-install/servicemesh-install.html

Requirements
------------

* OpenShift 3.11
* See supported configurations for more details:
  - https://docs.openshift.com/container-platform/3.11/servicemesh-install/servicemesh-install.html#supported-configurations

Setup
-----

The following Ansible variables should be defined:

```
openshift_master_public_url=<your master public url>
```

Deploy
------

Run the `install.yaml` Ansible playbook

```
ansible-playbook -i <inventory> install.yaml
```

License
-------

GPLv3

Author
------

Kevin Chung
