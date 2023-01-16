# Create Private GKE cluster
Ansible example for creating private GKE cluster

Requirements
------------
- Create project to host the cluster
- Generate SA account and download SA key to a location in `$HOME`
- update the `gcp_value.yaml` with the `service account ID` and `project ID`

Runing Ansible playbook
----------------
```bash
ansible-playbook gke.yaml # to create resources
ansible-playbook gke.yaml --extra-vars=remove_cluster=yes # to remove resources
```