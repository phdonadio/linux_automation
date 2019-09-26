## Linux System Installation Automation

The project is examples of unattended Linux distrobution installations using Packer.io and kickstart/preseed.

### Requirements

* Packer.io
* VirtualBox

### How To

* cd <distro>/
* packer build os_install.json


#### Notes

The automation files that drive the automated installation systems (i.e. kickstart and preseed) contains __plain text passwords__.  The project is designed to feed into CI/CD piplines.  The simple username/password combos are utlized to make it easier to feed into other automation consumers. The accounts should be hardened later in piplines designed to consume the resulting build artifacts from this project.
