### DICE code to run on updated Vagrant containers

# author: Mike Conway - DICE





















If you run into errors with VBox guest additions, use this sequence

If you not have vbguest plugin, install it:

$ vagrant plugin install vagrant-vbguest

The plugin github site is here: vg guest additions plugin that is required for that box image https://github.com/dotless-de/vagrant-vbguest




Log into host

sudo /etc/init.d/vboxadd setup 

And a vagrant reload later my guest was up and running again.

I'm just adding it here in case someone else gets here the same way I did.

It is possible that you get an error saying:

    The headers for the current running kernel were not found

This can be resolved by installing kernel-devel (yum install kernel-devel)



Run Vagrant

It is show a error.

$ vagrant up

Login on VM

$ vagrant ssh

Fix!

In the guest (VM logged).

$ sudo ln -s /opt/VBoxGuestAdditions-4.3.10/lib/VBoxGuestAdditions /usr/lib/VBoxGuestAdditions

Back on the host, reload Vagrant

$ vagrant reload


