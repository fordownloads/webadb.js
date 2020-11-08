## One-stop .js for Android Debug Bridge (adb) over WebUSB

```js
let webusb = await Adb.open("WebUSB");
let adb = await webusb.connectAdb("host::");
let shell = await adb.shell("uname -a");
console.log(await shell.receive());
```

## Install

From NPM:

```
npm install --save https://github.com/fordownloads/webadb.js
```

From yarn:

```
yarn add https://github.com/fordownloads/webadb.js
```
