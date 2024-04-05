# ansible-nfs

Modify configuration in roles/nfs/default/main.yml

Setup NFS Server:

ansible-playbook -i inventory playbook.yaml -l server -t nfs_server

Setup NFS Clients:

ansible-playbook -i inventory playbook.yaml -l clients -t nfs_client
# ansible-nfs
