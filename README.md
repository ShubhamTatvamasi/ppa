# ppa

https://launchpad.net/~shubhamtatvamasi

Upload your OpenPGP public key to: https://keyserver.ubuntu.com

Install `devscripts` for building debian packages:
```bash
sudo apt install devscripts
```

build the package:
```
dpkg-deb --build helloworld_1.0-1
```

upload package:
```bash
dput ppa:shubhamtatvamasi/hello helloworld_1.0-1.deb
```

Install package locally:
```bash
sudo apt install ./helloworld_1.0-1.deb
```

add repo to the on your system:
```bash
sudo add-apt-repository ppa:shubhamtatvamasi/hello
```
