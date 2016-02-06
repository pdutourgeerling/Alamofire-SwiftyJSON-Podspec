Updated Podspec for Alamofire-SwiftyJSON
==============
The current version of Alamofire-SwiftyJSON doesn't work with Swift 2.0 because it needs Alamofire 1.3, which doesn't support Swift 2.0. **This Podspec doesn't *force* any dependencies, but still *needs* them.** You need to add them manually like in the example below.

## Installation
To use this Podspec in your `Podfile` you must specify `:podspec` for the `Alamofire-SwiftyJSON` pod.
Make sure you have `pod 'Alamofire'` and `pod 'SwiftyJSON'` in your `Podfile` because you'll still need them.

## Example `Podfile` for Alamofire 2 (deprecated)
```ruby
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'
use_frameworks!

pod 'Alamofire', '~> 2.0.2'
pod 'SwiftyJSON'
pod 'Alamofire-SwiftyJSON', :podspec => 'https://raw.githubusercontent.com/pdutourgeerling/Alamofire-SwiftyJSON-Podspec/master/Alamofire-SwiftyJSON.podspec'
```

## Example `Podfile` for Alamofire 3
```ruby
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'
use_frameworks!

pod 'Alamofire', '~> 3.0'
pod 'SwiftyJSON'
pod 'Alamofire-SwiftyJSON', :podspec => 'https://raw.githubusercontent.com/pdutourgeerling/Alamofire-SwiftyJSON-Podspec/master/Alamofire3-SwiftyJSON.podspec'
```