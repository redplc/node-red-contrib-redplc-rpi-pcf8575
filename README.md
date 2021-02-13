# node-red-contrib-redplc-rpi-pcf8575

Node-Red node for pcf8575 16bit I/O Expander.<br>

## Node Features
- 2 x 8 x Digital Inputs or Digital Outputs
- Inputs with Pullup
- Outputs are Active Low
- Eight selectable Device Addresses

## Install

For using with Ladder-Logic install
[redPlc](https://www.npmjs.com/package/node-red-contrib-redplc) nodes

For using with other nodes, install
[module](https://www.npmjs.com/package/node-red-contrib-redplc-module) nodes

Install with Node-Red Palette Manager or npm command:
```
cd ~/.node-red
npm install node-red-contrib-redplc-rpi-pcf8575
```
## Usage
This node reads/writes from/to Node-Red global variables<br>
Update is triggered by redPlc cpu node or module-update node<br>
This node works only on Raspberry Pi with Raspberry Pi OS<br>
Enable I2C with raspi-config<br>
Consult datasheet for absolute maximum ratings<br>

### Digital Input (Variable I):
### Digital Output (Variable Q):

P0 = Input, P1 = Input<br>
P0 = Output, P1 = Output<br>

|Pin|Bit|Pin|Bit|
|:--|:-:|:--|:-:|
|P00|0|P10|8|
|P01|1|P11|9|
|P02|2|P12|10|
|P03|3|P13|11|
|P04|4|P14|12|
|P05|5|P15|13|
|P06|6|P16|14|
|P07|7|P17|15|

P0 = Input, P1 = Output<br>
P0 = Output, P1 = Input<br>

|Pin|Bit|Pin|Bit|
|:--|:-:|:--|:-:|
|P00|0|P10|0|
|P01|1|P11|1|
|P02|2|P12|2|
|P03|3|P13|3|
|P04|4|P14|4|
|P05|5|P15|5|
|P06|6|P16|6|
|P07|7|P17|7|

## Donate
If you like my work please support it with donate:

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZDRCZBQFWV3A6)
