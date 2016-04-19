**SSH Only Container for Tredly**

For Tredly-Build Version 0.9.0

**Installation**

This container requires Tredly-Host to build and run it, https://github.com/vuid-com/tredly-host

**Modifying container options**

By default, the container name is "sshonly". Change this by changing containerName in the Tredlyfile prior to building this container.

Many other options can be changed in the Tredlyfile

**Configuring SSH Only Container**

In the file sshd_config - add the external IP you wish to use. You could alternatively use Layer4Proxy and use the Tredly-Host external IP.

Add your ssh key into the authorised_key file

Modify Tredlyfile (Order of Operation section) so that the name of the user created for SSH access (root ssh access is bad practice) is to your liking. Currently the user is set to tredly.