# ansible-vmware-provisioning
ansible-playbook provisioning.yml --extra-vars=@./ocp4-upi-helpernode.yml --ask-vault-pass
# haproxy 
ansible-playbook provisioning-ocp4-haproxy.yml --extra-vars=@./ocp4-haproxy.yml --ask-vault-pass


# Delete cluster
ansible-playbook delete-cluster.yml --ask-vault-pass

ansible-playbook delete-ocp4-haproxy.yml --ask-vault-pass


