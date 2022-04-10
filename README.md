# install node-red 

(https://nodered.org/docs/getting-started/raspberrypi)
```
sudo apt install build-essential git curl -y
bash <(curl -sL https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered)
sudo systemctl enable nodered.service
sudo systemctl start nodered.service
```
### enable usb camera
```
sudo usermod -a -G video $USER

```
# teachable-node-red

```
git clone https://github.com/IBM/node-red-tensorflowjs
cd node-red-tensorflowjs
npm install
```

```
sudo apt install fswebcam -y
cd ~/.node-red
npm install ~/node-red-tensorflowjs/node-red-contrib-tfjs-object-detection/node-red-contrib-tfjs-object-detection
npm install node-red-contrib-browser-utils node-red-contrib-play-audio node-red-contrib-image-output 
npm install node-red-contrib-teachable-machine
```
