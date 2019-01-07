# Containers without Containers

A silly demonstration of faking containers in Linux by Mark Griffin <mark.griffin@linux.com>

This isn't even close to complete, but some idiot decided to run a tech talk at work, and didn't give himself enough time to set it up, so...

## Summary

This is not meant to be a serious platform, use Docker or something like normal people. That said, these scripts are mostly complete. They are designed to be used on a new CentOS 6 or 7 minimal installation. *I accept no responsibility for damage caused by these scripts.*


## Installation

*CentOS 6*
This uses chroot containerisation. Simply running the ./install script should do.

*CentOS 7*
This uses systemd containerisation. The /var/containers folder must be a btrfs mount.

