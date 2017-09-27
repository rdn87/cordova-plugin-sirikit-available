# cordova-plugin-sirikit-available

SiriKit Permission Cordova Plugin for iOS

Author: [Giulio Caruso aka rdn](https://twitter.com/giuliordn87)

[![Language](https://img.shields.io/badge/language-objective--c-green.svg)](https://developer.apple.com/reference/objectivec)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/rdn87/cordova-plugin-sirikit-available/blob/master/LICENSE)

## Adding the Plugin ##

Use the Cordova CLI and type in the following command:

`cordova plugin add https://github.com/rdn87/cordova-plugin-sirikit-available.git`

## Description

With this plug-in you can execute the native method `requestSiriAuthorization` for use *SiriKit*.

## Sample Code

The Plugin is only iOS Platform required iOS 10.0+.

### Execute requestPermission method in your Javascript

    cordova.plugins.requestPermission(function(response) {
        // success function
    }, function() {
        // failed function
    });
    
    response is flag (true/false) and identifies the state 
    true = INSiriAuthorizationStatusAuthorized
    false = INSiriAuthorizationStatusDenied, INSiriAuthorizationStatusNotDetermined, INSiriAuthorizationStatusRestricted
    
## License

cordova-plugin-sirikit-available is available under the MIT license. See the **[LICENSE](https://github.com/rdn87/cordova-plugin-sirikit-available/blob/master/LICENSE)** file for more info.
