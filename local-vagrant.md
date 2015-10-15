# local vagrant information

DFC is building a companion local vagrant install of DE components for developer work and maybe automated testing on a vanilla
configuration.

Under local-vagrant is a set of VMs, while it's a work in progress, we want to get to the point where one can run the de scripts and create a 'local' version with defaults.

## host info

We are standardizing a set of hosts that are reflected in the vagrant files under local-vagrant and the local-vagrant.yaml inventory

For convenience, you can copy these hosts into your own hosts conf for routing

192.168.50.10 cas.localvagrant.org
192.168.50.11 irods1.localvagrant.org
192.168.50.12 irods2.localvagrant.org



