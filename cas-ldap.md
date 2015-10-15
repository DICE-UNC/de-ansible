## Install and manage ldap and cas

For testing purposes, this script will install, configure, and manage an ldap and cas server, which can be provisioned with test users.  Currently, this should not be relied upon for production installs, it's for testing!

ansible-playbook cas-ldap.yml --inventory inventories/local-vagrant.yaml -K
