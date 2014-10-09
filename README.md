DWBubbleMenuButton
==================

![](demo.gif)

DWBubbleMenuButton is a simple animation framework for expanding and collapsing a variable sized menu. Project allows for expanding menus in left, right, up, and down directions. Using the framework is as simple as setting your home button and adding an array of menu buttons.

Usage
==================
Create a home a button
```objective-c
    UIButton *menuButton = [UIButton buttonWithType:UIButtonTypeSystem];

    [menuButton setTitle:@"Menu" forState:UIControlStateNormal];
```

Create an instance of DWBubbleMenuButton
```objective-c
    DWBubbleMenuButton *bubbleMenuButton = [[DWBubbleMenuButton alloc] initWithFrame:CGRectMake(20.f,
                                                                                            20.f,
                                                                                            100.f,
                                                                                            100.f)
                                                              expansionDirection:DirectionDown];
    bubbleMenuButton.homeButtonView = menuButton;
```

Add buttons to your bubble menu
```objective-c
    [bubbleMenuButton addButtons:@[ /* your buttons */]];
    
    /* OR */
    
    [bubbleMenuButton addButton:/* your button */];
```
