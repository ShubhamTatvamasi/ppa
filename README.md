# ppa

Install dput:
```bash
sudo apt install devscripts dput
```

build the package:
```
dpkg-deb --build helloworld_1.0-1
```

upload package:
```bash
dput ppa:shubhamtatvamasi/hello helloworld_1.0-1.deb
```

add repo to the on your system:
```bash
sudo add-apt-repository ppa:shubhamtatvamasi/hello
```
