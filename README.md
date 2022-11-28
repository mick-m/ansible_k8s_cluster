# Ansible playbook to deploy my K8S cluster

Instructions
------------
1.Bootstrap all nodes from inventory - e.g. :
```
$ ansible-playbook -u mick --ask-become-pass bootstrap.yml
```

2.Run role tasks  across cluster (base, k8s_controller, k8s_nodes)
```
$ ansible-playbook site.yml
```

Sources
-------
* Learn Linux TV video: Manually build a K8S cluster in [Proxmox](https://www.youtube.com/watch?v=U1VzcjCB_sY) (based on Ubuntue 22.04)
* Automated in Ansible taking some inspiration from [here](https://www.linuxsysadmins.com/install-kubernetes-cluster-with-ansible/).
