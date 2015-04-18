# rescue-live-image

This is a quite simple rescue system based on the Debian Live environment. It's base is a debian jessie minimal installation with some tools and ZFS from zfsonlinux.

Additional there is a kernel commandline option to supply the system with a public ssh key for the root account. This can be used by adding:
root-ssh-key="[KEY]" to the kernel parameters, where [KEY] is your public ssh key as you would add it to ~/.ssh/authorized_keys.

To build the system just install debian-live. Then run:
lb config
sudo lb build

For further documentation on the Debian Live build process refer to http://live.debian.net/
