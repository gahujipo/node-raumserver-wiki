# Manual install on a Linux operating system

## Installing NodeJS
Please use with node version 7.x or above. You can do that by using [nodesource.com]()s bash script that you can directly download and launch by issuing the follwoing commands: 

```bash
curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
sudo apt install nodejs
```
or if you prefer for version 8 of nodejs
```bash
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt-get install nodejs
```

With the installation comes npm, **N**odeJSs **P**acket **M**anager. We will use npm to install node-raumserver itself.

## Installing node-raumserver package

```bash
cd <directory you want to install node-raumserver to>
npm install github:ChriD/node-raumserver
```

## Start node-raumserver
```bash
cd <directory you installed node-raumserver to>
node raumserver.js
```
node-raumserver will startup and use port 8080 , which is the default port. You can change that in the file [config/default.json](../Config.md)