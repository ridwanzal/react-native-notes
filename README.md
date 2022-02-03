# List react-native development notes
Useful notes for end to end development with react-native

## Installation

### 1. Problem when install react native using npx
Remove npm cache, and install npm package globally with stable version, and you good to go

```
$ sudo npm cache clean -f
$ sudo npm install -g n
$ sudo n stable
```
### 2. Set local properties 
When using android emulator place local properties inside 
{react-project-name}/android

Create local propertis
```
$ sudo touch local.properties
```

Add android sdk path to *local.properties*
```
sdk.dir = /home/ridwanzal/Android/Sdk/
```
### 3. Run AVD from Sdk Library path
Make sure at least you have on active AVD installed on your system that can run on react-native project
```
$ cd /home/ridwanzal/Android/Sdk/emulator
```

```
$user:/home/ridwanzal/Android/Sdk/emulator# ./emulator -list-avds
Pixel_4_XL_API_30
```

Run AVD with following command :
```
./emulator -avd Pixel_4_XL_API_30
```

## Running react-native app on AVD
When your AVD is already running you can run the following command, to build and run react-native app to AVD
```
$ npx react-native start
```
