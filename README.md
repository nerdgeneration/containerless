# Containers without Containers

A silly demonstration of faking containers in Linux.

This isn't even close to complete, but some idiot decided to run a tech talk at work*, and didn't give himself enough time to set it up, so...

(* see Containers without Containers.odp)


## Summary

This is not meant to be a serious platform, use Docker or something like normal people.

If you want to use these scripts, they are designed to be used on a new CentOS 6 or 7 minimal installation.

**I accept no responsibility for damage caused by these scripts (especially because they're incomplete right now).**


## Installation

**CentOS 6**: This uses chroot containerisation. Simply running the ./install script should do.

**CentOS 7**: This uses systemd containerisation. The /var/containers folder must be a btrfs mount (which you must do yourself), then run the ./install script.

**CentOS 8**: This is currently a symlink to CentOS 6 because 8 doesn't have btrfs support.

The install script disables SELinux, installs some packages, does an update and pushes the scripts to /usr/local/bin.


## Usage

**container-create name size**: Creates a base image and puts you in a shell to configure it.

**container-destroy name**: Does nothing, but does leave a little advice on doing it manually. You're welcome :)

**container-deploy name deploy-name on|off**: Very much work in progress. Consider this pseudo-code for now.

Documentation is this page and the source code.


## Future

If you come back next month, this might be more complete. It's about time I did more open source stuff, even if it is effectively useless.

```
/* @author Mark Griffin <mark.griffin@linux.com> */
```