Stand alone nvme driver modified from the original Centos 7.3 sources.  Allows for longer admin command timeouts.


Ensure all kernel-devel dependencies are installed.  Requires system ignores kernel module signing, disable Secure Boot or be prepared to sign module.

Build:
$ make

Install:
$ sudo insmod nvme/host/nvme.ko admin_timeout=1600


