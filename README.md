HTPressableButton
==============
HTPressableButton is designed for iOS developers to be able to focus more on other tasks instead of making a pretty button. It has a Flat UI design and is very easy to integrate.


Installation
-------------------
HTPressableButton can be installed via [Cocoapods](http://cocoapods.org/)

```ruby
pod 'HTPressableButton'
```

Another option is to use git submodules or just [download it](https://github.com/Grouper/FlatUIKit/archive/master.zip) and include it in your project manually.

**NOTE:** Please be reminded to add the header file when implementing

```objective-c
#import "HTPressableButton.h"
#import "UIColor+HTColor.h"
```

The second header file is not needed if you do not wish to use the Flat UI colors provided, but only use the default UIColors given by Apple.

Components
-------------------
###Rectangle Button
```objective-c
    HTPressableButton *rectButton = [HTPressableButton buttonWithType:UIButtonTypeCustom];
    rectButton.frame = CGRectMake(30, 150, 260, 50);
    rectButton.buttonColor = [UIColor grapeFruitColor];
    rectButton.shadowColor = [UIColor grapeFruitDarkColor];
    rectButton.style = rect;
    [rectButton setTitle:@"Rect" forState:UIControlStateNormal];
    [self.view addSubview:rectButton];
```

![HTPressableButton](https://raw.githubusercontent.com/herinkc/HTPressableButton/master/READMEImages/RectButtonImage.gif?token=3966522__eyJzY29wZSI6IlJhd0Jsb2I6aGVyaW5rYy9IVFByZXNzYWJsZUJ1dHRvbi9tYXN0ZXIvUkVBRE1FSW1hZ2VzL1JlY3RCdXR0b25JbWFnZS5naWYiLCJleHBpcmVzIjoxMzk4OTY0NDg0fQ%3D%3D--f8882a05961b42509cb76cadc33bff716248e584)


###Rounded Rectangle Button
```objective-c
    HTPressableButton *roundedRectButton = [HTPressableButton buttonWithType:UIButtonTypeCustom];
    roundedRectButton.frame = CGRectMake(30, 230, 260, 50);
    roundedRectButton.style = rounded;
    [roundedRectButton setTitle:@"Rounded" forState:UIControlStateNormal];
    [self.view addSubview:roundedRectButton];
```

![HTPressableButton](https://raw.githubusercontent.com/herinkc/HTPressableButton/master/READMEImages/RoundedRectButtonImage.gif?token=3966522__eyJzY29wZSI6IlJhd0Jsb2I6aGVyaW5rYy9IVFByZXNzYWJsZUJ1dHRvbi9tYXN0ZXIvUkVBRE1FSW1hZ2VzL1JvdW5kZWRSZWN0QnV0dG9uSW1hZ2UuZ2lmIiwiZXhwaXJlcyI6MTM5ODk2NDYzMn0%3D--4049b9f971c220426b67c8e6b812d6a163a04e8a)


###Circle Button
```objective-c
    HTPressableButton *circleButton = [HTPressableButton buttonWithType:UIButtonTypeCustom];
    circleButton.frame = CGRectMake(110, 300, 100, 100);
    circleButton.style = circle;
    circleButton.buttonColor = [UIColor mintColor];
    circleButton.shadowColor = [UIColor mintDarkColor];
    [circleButton setTitle:@"Circle" forState:UIControlStateNormal];
    [self.view addSubview:circleButton];
```

![HTPressableButton](https://raw.githubusercontent.com/herinkc/HTPressableButton/master/READMEImages/CircleButtonImage.gif?token=3966522__eyJzY29wZSI6IlJhd0Jsb2I6aGVyaW5rYy9IVFByZXNzYWJsZUJ1dHRvbi9tYXN0ZXIvUkVBRE1FSW1hZ2VzL0NpcmNsZUJ1dHRvbkltYWdlLmdpZiIsImV4cGlyZXMiOjEzOTg5NjQ2MTN9--c1d65c71dbeed8a9f83db8073114f06caef80e53)


**NOTE:** If you do not choose *button.style*, the default will be a rectangle button.


License
-------------------
This projected is licensed under the terms of the [MIT license](https://github.com/herinkc/HTPressableButton/blob/master/LICENSE).