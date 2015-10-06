## Install and manage iRODS servers

For testing purposes, this script will install, configure, and manage a pair of federated iRODS servers

ansible-playbook irods.yml --check --inventory inventories/renci.yaml --extra-vars "irods_passwd=xxx icat_password=xxxx" -K

FIXME: IOError: [Errno 2] No such file or directory: '/var/lib/irods/.odbc.ini'

