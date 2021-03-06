# Set Geolocation

Set the current geo location
## Example Usage

```java
// Java
driver.setLocation(new Location(49, 123, 10)); // Must be a driver that implements LocationContext

```

```python
# Python
self.driver.set_location(49, 123, 10)

```

```javascript
// Javascript
// webdriver.io example
driver.location({latitude: 121.21, longitude: 11.56, altitude: 94.23});



// wd example
let location = await driver.sessionCapabilities('c8db88a0-47a6-47a1-802d-164d746c06aa');

```

```ruby
# Ruby
@driver.set_location(121.21, 11.56, 94.23)

```

```php
# PHP
// TODO PHP sample

```

```csharp
// C#
// TODO C# sample

```



## Support

### Appium Server

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
| iOS | [XCUITest](/docs/en/drivers/ios-xcuitest.md) | 9.3+ | 1.6.0+ | All |
|  | [UIAutomation](/docs/en/drivers/ios-uiautomation.md) | 8.0 to 9.3 | All | All |
| Android | [UiAutomator2](/docs/en/drivers/android-uiautomator2.md) | ?+ | 1.6.0+ | All |
|  | [UiAutomator](/docs/en/drivers/android-uiautomator.md) | 4.2+ | All | All |
| Mac | [Mac](/docs/en/drivers/mac.md) | ?+ | 1.6.4+ | All |
| Windows | [Windows](/docs/en/drivers/windows.md) | 10+ | 1.6.0+ | All |

### Appium Clients

|Language|Support|Documentation|
|--------|-------|-------------|
|[Java](https://github.com/appium/java-client/releases/latest)| All |  [seleniumhq.github.io](https://seleniumhq.github.io/selenium/docs/api/java/org/openqa/selenium/html5/LocationContext.html#location--)  |
|[Python](https://github.com/appium/python-client/releases/latest)| All |  [selenium-python.readthedocs.io](http://selenium-python.readthedocs.io/api.html)  |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| All |  [webdriver.io](http://webdriver.io/api/protocol/location.html)  |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| All |  [github.com](https://github.com/admc/wd/blob/master/lib/commands.js#L407)  |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| All |  [www.rubydoc.info](http://www.rubydoc.info/gems/selenium-webdriver/Selenium%2FWebDriver%2FDriverExtensions%2FHasLocation:set_location)  |
|[PHP](https://github.com/appium/php-client/releases/latest)| All |  [github.com](https://github.com/appium/php-client/)  |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| All |  [github.com](https://github.com/appium/appium-dotnet-driver/)  |

## HTTP API Specifications

### Endpoint

`POST /session/:session_id/location`

### URL Parameters

|name|description|
|----|-----------|
|session_id|ID of the session to route the command to|

### JSON Parameters

|name|type|description|
|----|----|-----------|
| latitude | `number` | The current geolocation latitude |
| longitude | `number` | The current geolocation longitude |
| altitude | `number` | The current geolocation altitude |

### Response

null

## See Also

* [JSONWP Specification](https://github.com/SeleniumHQ/selenium/wiki/JsonWireProtocol#post-sessionsessionidlocation)
