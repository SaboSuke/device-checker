# Device Checker

[![Software Version](https://img.shields.io/badge/device--checker-v1.0.0-green)](https://github.com/SaboSuke/device-checker)

A simple library to check if the current device is mobile or tablet.

## Options

Name | Type | Default | Explanation
---- | ---- | ------- | -----------
  `addToWindow` | `Boolean` | `false` | Should the methods be added to the window object.

## Methods

Name | Returns | Explanation
---- | ------- | -----------
  `isMobileOrTablet` | `Boolean` | Check if the current device is mobile or tablet.
  `isMobile` | `Boolean` | Check if the current device is mobile.
  `detectMobile` | `Boolean` | Detect a mobile device based on a list of devices from the `MOBILE_DEVICES` constant or an array of devices of your chosing.

## Usage

```javascript

// basic usage
const isMobile = new DeviceChecker().isMobile();
const isMobileOrTablet = new DeviceChecker().isMobileOrTablet();

// you can also add the methods to the window object like so
const checker = new DeviceChecker({
    addToWindow: true
});

if(window.isMobileOrTablet){
    // do something
}

```

## Contributing

If you have anything to contribute, or functionality that you lack - you are more than welcome to participate in this!
If anyone wishes to contribute unit tests that also would be great.

## License

The MIT License (MIT)

Copyright (c) 2021 Essam Abed (abedissam95@gmail.com)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.