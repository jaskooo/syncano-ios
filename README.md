[![Circle CI](https://circleci.com/gh/Syncano/syncano-ios/tree/master.svg?style=svg)](https://circleci.com/gh/Syncano/syncano-ios/tree/master)

# Syncano iOS Library

## Overview
---

Syncano's iOS library is written in Objective-C and provides communication with Syncano ([www.syncano.io](http://www.syncano.io/?utm_source=github&utm_medium=readme&utm_campaign=syncano-ios)) via HTTPS RESTful interface.

The full source code can be found on [Github](https://github.com/Syncano/syncano-ios) - feel free to browse or contribute.

## iOS QuickStart Guide
---

You can find quick start on installing and using Syncano's iOS library (for both Obj-C and Swift) in our [documentation](http://docs.syncano.com/docs/ios/?utm_source=github&utm_medium=readme&utm_campaign=syncano-ios).

For more detailed information on how to use Syncano and its features - our [Developer Manual](http://docs.syncano.com/docs/getting-started-with-syncano/?utm_source=github&utm_medium=readme&utm_campaign=syncano-ios) should be very helpful.

In case you need help working with the library - email us at libraries@syncano.com - we will be happy to help!

## Documentation
-------------

 Appledoc documentation can be generated by building a `Documentation` target in `syncano-ios.xcworkspace`. Docs will be in the `Syncano-Docs` directory and will be installed to the Xcode documentation, too. In case something is wrong, logs are put into the `appledoc.log` file. If you need to download `appledoc` visit [https://github.com/tomaz/appledoc/](https://github.com/tomaz/appledoc/).

To write documentation, we recommend using the [`VVDocumenter` XCode plugin](https://github.com/onevcat/VVDocumenter-Xcode). It makes writing correctly structured documentation a little easier. Simply place your cursor above method/class/anything you wish to describe, and type `///` to generate a documentation template snippet for that item.

## License
---

Syncano's iOS Library (syncano-ios) is available under the MIT license. See the LICENSE file for more info.

## Change Log
--
* **4.0.12** - 2016-02-18
    * Fixed bug with social backends login 
* **4.0.11** - 2016-02-17
    * Fixed saving objects with empty relations
    * Fixed saving files to disks memory management issue
    * Added missing predicates for working with local storage
* **4.0.10** - 2016-02-12
    * Fixed using custom class for User and User Profile 
* **4.0.9** - 2016-02-11
    * Offline storage (save results to offline and query local storage)
    * Added string filtering on objects (contains, startsWith, endsWith - both case sensitive and insensitivie)
    * Handling custom responses in CodeBoxes and Webhooks
    * Fix for default permissions (now by default permissions are .NotSet - taking defaults from the server)
    * Fix for properly transforming `updated_at` and `created_at` fields from string to `NSDate` 
    * Added ability to save files (`SCFile`) to disk
    * Added SSL certificate  
    * Implemented Data Views
    * Added Twitter/LinkedIn login
    * More powerful filtering (filter by properties of classes, that one class has reference to)
    * Added ability to incerement fields (helps with concurrency when updating objects) 
* **4.0.8** - 2016-02-10
    * Fixed issue with fetching SCFile content 
* **4.0.7** - 2016-01-29
    * Fixed default owner permissions when creating a new object
* **4.0.6** - 2015-12-01
    * Fixed webhook payload wraping
    * Added framework targed instead of static library in xcode project
    * Added documentation target
    * Added pages enumerator to SCPlease
    * Removed automatic reference objects fetching
    * Removed SCPleaseParameterIncludeKey
    * Updated AFNetworking to 2.6.3
