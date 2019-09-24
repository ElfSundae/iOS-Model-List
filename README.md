# iOS Model List

📱 The ultimate list of iOS device models - Identify your iPhone, iPad, iPod touch, ⌚️ Apple Watch, 🖥 Apple TV model.

:rocket: Capturing the latest model list at https://0x123.com/iOS-Model-List/

## List Preview:

```json
{
  "AppleTV2,1": "Apple TV 2",
  "AppleTV3,1": "Apple TV 3",
  "AppleTV3,2": "Apple TV 3",
  "AppleTV5,3": "Apple TV 4",
  "AppleTV6,2": "Apple TV 4K",
  "iPad1,1": "iPad",
  "iPad2,1": "iPad 2",
  "iPad2,2": "iPad 2",
  "iPad2,3": "iPad 2",
  "iPad2,4": "iPad 2",
  "iPad2,5": "iPad mini",
  "iPad2,6": "iPad mini",
  "iPad2,7": "iPad mini",
  "iPad3,1": "iPad 3",
  "iPad3,2": "iPad 3",
  "iPad3,3": "iPad 3",
  "iPad3,4": "iPad 4",
  "iPad3,5": "iPad 4",
  "iPad3,6": "iPad 4",
  "iPad4,1": "iPad Air",
  "iPad4,2": "iPad Air",
  "iPad4,3": "iPad Air",
  "iPad4,4": "iPad mini 2",
  "iPad4,5": "iPad mini 2",
  "iPad4,6": "iPad mini 2",
  "iPad4,7": "iPad mini 3",
  "iPad4,8": "iPad mini 3",
  "iPad4,9": "iPad mini 3",
  "iPad5,1": "iPad mini 4",
  "iPad5,2": "iPad mini 4",
  "iPad5,3": "iPad Air 2",
  "iPad5,4": "iPad Air 2",
  "iPad6,3": "iPad Pro (9.7-inch)",
  "iPad6,4": "iPad Pro (9.7-inch)",
  "iPad6,7": "iPad Pro (12.9-inch)",
  "iPad6,8": "iPad Pro (12.9-inch)",
  "iPad6,11": "iPad 5",
  "iPad6,12": "iPad 5",
  "iPad7,1": "iPad Pro 2 (12.9-inch)",
  "iPad7,2": "iPad Pro 2 (12.9-inch)",
  "iPad7,3": "iPad Pro 2 (10.5-inch)",
  "iPad7,4": "iPad Pro 2 (10.5-inch)",
  "iPad7,5": "iPad 6",
  "iPad7,6": "iPad 6",
  "iPad8,1": "iPad Pro 3 (11-inch)",
  "iPad8,2": "iPad Pro 3 (11-inch)",
  "iPad8,3": "iPad Pro 3 (11-inch)",
  "iPad8,4": "iPad Pro 3 (11-inch)",
  "iPad8,5": "iPad Pro 3 (12.9-inch)",
  "iPad8,6": "iPad Pro 3 (12.9-inch)",
  "iPad8,7": "iPad Pro 3 (12.9-inch)",
  "iPad8,8": "iPad Pro 3 (12.9-inch)",
  "iPad11,1": "iPad mini 5",
  "iPad11,2": "iPad mini 5",
  "iPad11,3": "iPad Air 3",
  "iPad11,4": "iPad Air 3",
  "iPhone1,1": "iPhone",
  "iPhone1,2": "iPhone 3G",
  "iPhone2,1": "iPhone 3GS",
  "iPhone3,1": "iPhone 4",
  "iPhone3,2": "iPhone 4",
  "iPhone3,3": "iPhone 4",
  "iPhone4,1": "iPhone 4S",
  "iPhone5,1": "iPhone 5",
  "iPhone5,2": "iPhone 5",
  "iPhone5,3": "iPhone 5c",
  "iPhone5,4": "iPhone 5c",
  "iPhone6,1": "iPhone 5s",
  "iPhone6,2": "iPhone 5s",
  "iPhone7,1": "iPhone 6 Plus",
  "iPhone7,2": "iPhone 6",
  "iPhone8,1": "iPhone 6s",
  "iPhone8,2": "iPhone 6s Plus",
  "iPhone8,4": "iPhone SE",
  "iPhone9,1": "iPhone 7",
  "iPhone9,2": "iPhone 7 Plus",
  "iPhone9,3": "iPhone 7",
  "iPhone9,4": "iPhone 7 Plus",
  "iPhone10,1": "iPhone 8",
  "iPhone10,2": "iPhone 8 Plus",
  "iPhone10,3": "iPhone X",
  "iPhone10,4": "iPhone 8",
  "iPhone10,5": "iPhone 8 Plus",
  "iPhone10,6": "iPhone X",
  "iPhone11,2": "iPhone XS",
  "iPhone11,4": "iPhone XS Max",
  "iPhone11,6": "iPhone XS Max",
  "iPhone11,8": "iPhone XR",
  "iPhone12,1": "iPhone 11",
  "iPhone12,3": "iPhone 11 Pro",
  "iPhone12,5": "iPhone 11 Pro Max",
  "iPod1,1": "iPod touch",
  "iPod2,1": "iPod touch 2",
  "iPod3,1": "iPod touch 3",
  "iPod4,1": "iPod touch 4",
  "iPod5,1": "iPod touch 5",
  "iPod7,1": "iPod touch 6",
  "iPod9,1": "iPod touch 7",
  "Watch1,1": "Apple Watch (38mm)",
  "Watch1,2": "Apple Watch (42mm)",
  "Watch2,3": "Apple Watch Series 2 (38mm)",
  "Watch2,4": "Apple Watch Series 2 (42mm)",
  "Watch2,6": "Apple Watch Series 1 (38mm)",
  "Watch2,7": "Apple Watch Series 1 (42mm)",
  "Watch3,1": "Apple Watch Series 3 (38mm, LTE)",
  "Watch3,2": "Apple Watch Series 3 (42mm, LTE)",
  "Watch3,3": "Apple Watch Series 3 (38mm)",
  "Watch3,4": "Apple Watch Series 3 (42mm)",
  "Watch4,1": "Apple Watch Series 4 (40mm)",
  "Watch4,2": "Apple Watch Series 4 (44mm)",
  "Watch4,3": "Apple Watch Series 4 (40mm, LTE)",
  "Watch4,4": "Apple Watch Series 4 (44mm, LTE)",
  "Watch5,1": "Apple Watch Series 5 (40mm)",
  "Watch5,2": "Apple Watch Series 5 (44mm)",
  "Watch5,3": "Apple Watch Series 5 (40mm, LTE)",
  "Watch5,4": "Apple Watch Series 5 (44mm, LTE)",
  "i386": "Simulator",
  "x86_64": "Simulator"
}
```

## Code Examples

- Objective-C code `-[UIDevice modelName]` from [ESFramework](https://github.com/ElfSundae/ESFramework/blob/master/ESFramework/UIKit/UIDevice%2BESExtension.m#L86):

    ```objc
    - (NSString *)modelName
    {
        static NSString *_modelName = nil;
        static dispatch_once_t onceToken;
        dispatch_once(&onceToken, ^{
            NSDictionary *models = @{

                // MARK: Put The List Here...

                @"AppleTV2,1": @"Apple TV 2",
                @"AppleTV3,1": @"Apple TV 3",
                @"iPad1,1": @"iPad",
                @"iPad2,1": @"iPad 2",
            };
            _modelName = models[self.modelIdentifier] ?: self.modelIdentifier;
        });
        return _modelName;
    }
    ```

## References

- [Models - The iPhone Wiki](https://www.theiphonewiki.com/wiki/Models)
- [Identify your iPhone model - Apple Support](https://support.apple.com/en-us/HT201296)
- [Identify your iPad model - Apple Support](https://support.apple.com/en-us/HT201471)
- [Identify your iPod model - Apple Support](https://support.apple.com/en-us/HT204217)
- [Identify your Apple Watch - Apple Support](https://support.apple.com/en-us/HT204507)
- [Identify your Apple TV model - Apple Support](https://support.apple.com/en-us/HT200008)
- [IPSW Downloads API](https://ipswdownloads.docs.apiary.io/#reference/api/devices/v-4-.-get-devices)
