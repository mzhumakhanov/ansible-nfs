# ansible-nfs

Modify configuration in roles/nfs/default/main.yml and hosts in file "inventory".

By this moment only one NFS server will be used - the first from group "server".
Meanwhile it's possible to specify new server for an every new run.

The list of NFS clients in inventory can be defined without limitations.

Setup NFS Server:

ansible-playbook -i inventory playbook.yaml -l server -t nfs_server

Setup NFS Clients:

ansible-playbook -i inventory playbook.yaml -l clients -t nfs_client
