## Chengcheng Xiao's ports
This is a portfile repository maintained by Chengcheng Xiao.

## Usage
Following [the official guide](https://guide.macports.org/chunked/development.local-repositories.html) clone this repository to your local machine
```
git clone git@github.com:Chengcheng-Xiao/.macports.git
```
then add the following line to `/opt/local/etc/macports`:
```
file:///Users/USER_NAME/.macports/ports
```
Then go to `/Users/USER_NAME/.macports/ports` to index the ports
```
portindex
```
Finally allow macports to search the ports (because of [macOS ACLs](https://macports-users.macosforge.narkive.com/oLdhXnu6/fail-to-execute-a-custom-local-portfile))
```
chmod +a 'macports allow search' ~ 
```
you can revserse this by 
```
chmod -a "macports allow search" ~
```

## Install ports
Simply install ports using macports
```
sudo port install PORT_NAME
```
