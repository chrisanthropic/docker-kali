## WHAT
Use this file to create a base Kali Linux image for docker.

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

Once it's finsihed run `docker images` and you should see it listed as blackfinsecurity/kali.
