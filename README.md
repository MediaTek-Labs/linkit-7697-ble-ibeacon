# LinkIt 7697 BLE iBeacon
How to use BLE to emulate iBeacon on LinkIt 7697 HDK

Additinal resource can be found at https://docs.labs.mediatek.com/resource/mt7687-mt7697

## Folder Structure

* `project/linkit7697_hdk/apps/ble_ibeacon`: LinkIt SDK project files.

## How to Build

### Device Side

* Put/Extract the files into SDK root, so that there is `[SDK_root]/project/linkit7697_hdk/apps/ble_ibeacon`
* Execute `./build.sh linkit7697_hdk ble_ibeacon` under Linux enviornment
* Check generated bin at `[SDK_root]/out/linkit7697_hdk/ble_ibeacon/ble_ibeacon.bin`
* Use Flashtool to download `[SDK_root]/out/linkit7697_hdk/ble_ibeacon/flash_download.ini` into LinkIt 7697 HDK

### Mobile Side

* Install any beacon app (ex. Locate Beacon app)

## How to Run

### Phases

* Turn on Device, when it is ready, it will start "BLE Advertising"

### Mobile Side

![Mobile](/images/mobile.png)

### Device Side

Below are log output from UART port of LinkIt 7697 HDK
![Device](/images/device.png)

## Message Sequence Chart

![MSC](/images/msc.png)


