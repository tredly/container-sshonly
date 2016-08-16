## SSH Only Container for Tredly

Version 1.0.4 August 16 2016

## Installation

Requires Tredly 1.1.0 <https://github.com/tredly/tredly> or later

## Modifying container options**

By default, the container name is "sshonly". Change this by changing containerName in `tredly.yaml` prior to building this container.

Many other options can be changed in `tredly.yaml`

## Configuring SSH Only Container**

In the file `sshd_config` - add the external IP you wish to use. You could alternatively use Layer4Proxy and use the Tredly host external IP.

Add your ssh key into the `authorized_keys` file

Modify `tredly.yaml` (Order of Operation section) so that the name of the user created for SSH access (root ssh access is bad practice) is to your liking. Currently the user is set to `tredly`.

## License

Tredly is released under the [MIT License](http://www.opensource.org/licenses/MIT).
