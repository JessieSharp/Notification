# Notification

Material design notify system for WPF applications

## Getting Started

- Build Notification project for the .dll
- Add Notification.dll reference in your application
- Copy MaterialDesignColor.dll and MaterialDesignThemes.Wpf.dll from build folder to your app folder

- Add namespace
```
using Notifications;
```

- Create main object
```
private readonly Main _notify = new Main();
```

- In your init method add
```
public MainWindow()
{
    InitializeComponent();
    _notify.PrepareWindow();
}
```

- Finally you can call the function
```
_notify.ShowNotify(Main.NotifyType.Error, "Title", "Description");
```

**Important**
Before user close the application you should call 
```
_notify.KillWindow();
```
if you don't do this process will be still in memory!
### Screenshots

![Alt text](https://i.imgur.com/V594W3V.png "Optional title")
![Alt text](https://i.imgur.com/zgYcHWv.gif "Optional title")
