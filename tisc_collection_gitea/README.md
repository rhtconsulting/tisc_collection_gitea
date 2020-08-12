# Ansible Collection - rht_consulting.tisc_collection_gitea

Documentation for the collection.

The following example playbook will import and execute this collection

```
---
- hosts: localhost
  tasks:
    - import_role:
        name: rht_consulting.tisc_collection_gitea.gitea
```

To run this the following vars need to be defined

p_cluster_name
p_base_domain
p_kube_config
p_oc_cli

For example, if the playbook above is named play.yml and our ocp cluster domain is openshift.example.net the youcan un the following to launch the collection

ansible-playbook -e 'p_cluster_name=openshift p_base_domain=openshift.example.net p_kube_config=<OCP_INSTALL_DIR>/auth/kubeconfig p_oc_cli=/usr/local/bin/oc' play.yml
