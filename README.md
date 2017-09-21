# Kathará
Implementation of the notorious [Netkit](https://github.com/maxonthegit/netkit-core) using Python and Docker, allowing for SDN, NFV and traditional routing protocols. Comes with P4, Bind, Quagga, OpenVSwitch and more. 

Kathará has the performances to run in production and can emulate most network equipments. 

## Installation
* To run Kathará you first need to install [Docker](https://www.docker.com/) and Python 2.x.
* Download all the files to a directory of your choice.
* Add the environment variable NETKIT_HOME to your system pointing to the bin folder:
  * Unix: `export NETKIT_HOME=/home/foo/kathara/bin`
  * Windows: System > Advanced settings > Environment Variables > New > ...
* Run the installer:
  * Unix: `$NETKIT_HOME/install`
  * Windows: `%NETKIT_HOME%\install`
* You can optionally add NETKIT_HOME to your PATH

# Manual
The interface of Kathará is basically the same we used for Netkit, and it's available here: [Man page of NETKIT](http://wiki.netkit.org/man/man7/netkit.7.html).

The main difference is the way we specify the interfaces in the `vstart` command (now requiring `--eth 0:A --eth 1:B ...`) but why would you ever use `vstart` when you have `lstart`?
