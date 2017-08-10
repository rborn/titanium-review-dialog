## SKStoreReviewController (iOS 10.3+) in Appcelerator Titanium
[![Build Status](https://travis-ci.org/hansemannn/titanium-review-dialog.svg?branch=master)](https://travis-ci.org/hansemannn/titanium-review-dialog) [![License](http://hans-knoechel.de/shields/shield-license.svg?v=1)](./LICENSE) [![Contact](http://hans-knoechel.de/shields/shield-twitter.svg?v=1)](http://twitter.com/hansemannnn)

<img src="example/example-screen.png" width="320" alt="Example" />

### Summary
Use the `SKStoreReviewController` from iOS 10.3+ in your Ttanium application.

### Requirements
  - Titanium Mobile SDK 6.0.0.GA or later
  - iOS 10.3 or later
  - Xcode 8.3 or later

### Download
  * [Stable release](https://github.com/hansemannn/titanium-review-dialog/releases)
  * [![gitTio](http://hans-knoechel.de/shields/shield-gittio.svg)](http://gitt.io/component/ti.reviewdialog)

### Setup
Unpack the module and place it inside the `modules/iphone/` folder of your project.
Edit the modules section of your `tiapp.xml` file to include this module:
```xml
<modules>
    <module platform="iphone">ti.reviewdialog</module>
</modules>
```

### Hyperloop
This module is also built in Hyperloop to demonstrate the native API access with JavaScript.
You can simple require the `ti.reviewdialog.js` in your application and run it!

### Example
Request a new review dialog:
```javascript
var Review = require('ti.reviewdialog');

if (Review.isSupported()) {
  Review.requestReview();
}
```
#### Methods
- [x] `isSupported`
- [x] `requestReview`

### Author
Hans Knoechel ([@hansemannnn](https://twitter.com/hansemannnn) / [Web](http://hans-knoechel.de))

### License
Apache 2.0

### Contributing
Code contributions are greatly appreciated, please submit a new [pull request](https://github.com/hansemannn/titanium-review-dialog/pull/new/master)!
