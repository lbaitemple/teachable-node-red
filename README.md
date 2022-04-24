# install nodejs
```
curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -
sudo apt-get install -y nodejs

```

# install node-red 

(https://nodered.org/docs/getting-started/raspberrypi)
```
sudo apt update && sudo apt upgrade -y
sudo apt install build-essential git curl -y
bash <(curl -sL https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered)
sudo systemctl enable nodered.service
sudo systemctl start nodered.service
```
### enable usb camera
```
sudo usermod -a -G video $USER

```

### teachable-node-red
```
sudo apt install fswebcam -y
cd ~/.node-red
npm install node-red-contrib-browser-utils node-red-contrib-play-audio node-red-contrib-image-output  node-red-contrib-usbcamera  
npm install @tensorflow/tfjs 
npm install node-red-contrib-teachable-machine
```

#### choose USB_camera
<img src="usb_camera.png" width="448">
You will need to choose generate before use buffer option
#### may needed.....

## install dependencies
```
cd ~
git clone https://github.com/IBM/node-red-tensorflowjs
cd ~/node-red-tensorflowjs
npm install
cd ~/.node-red
npm install ~/node-red-tensorflowjs/node-red-contrib-tfjs-object-detection/node-red-contrib-tfjs-object-detection

