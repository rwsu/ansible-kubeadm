# Ansible Kubeadm and Gluster/Heketi Installer

## Overview

This repository contains playbooks to

* install a Kubernetes cluster on baremetal servers using kubeadm and Flannel as the CNI 
* install GlusterFS and Heketi
* uninstall Kubernetes and associated packages

## Usage

To install Kubernetes run this command:

```
ansible-playbook -i inventory provision.yml
```

After Kubernetes has been installed, install GlusterFS and Heketi by:

```
ansible-playbook -i inventory gluster.yml
```

To uninstall
```
ansible-playbook -i inventory deprovision.yml
```
