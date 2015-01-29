## WHAT
Use this file to create a base Kali Linux image for docker.

This install uses the [kali-linux](https://www.kali.org/news/kali-linux-metapackages/) metapackage from Kali, so it's very very stripped down and is essentially just the Kali desktop with git and ssh and a few other tools.
You can install the other tools via apt-get or using Kali's other metapackages.

## WHY
Kali Linux is primarily used for security training/testing. Don't trust other people to build your docker-kali image, build your own.

## HOW

*NOTE:* This script requires debootstrap, so however you install stuff on your distro make sure you install it before trying to run this script.

From a linux cli:
```
git clone https://github.com/ctarwater/docker-kali.git
cd docker-kali
./build.sh
```

Once it's finsihed run `docker images` and you should see it listed as ctarwater/kali.
