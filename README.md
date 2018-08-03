# EasySnackBar
A SnackBar can show at top and bottom with a custom layout.

This a SnackBar focuse on show custom layout,so it will not provide the same interface as the Google'Snackbar.

#### Notice
This Snackbar must be used in same environment as the google's Snackbar, otherwise it will show in wrong case.
For example, it's should be shown in a CoordinatorLayout.

#### The effect show as the GIF below

![demo](https://github.com/SunJenry/EasySnackBar/blob/master/cq382-3pv13.gif)


#### Usage

1. Adding dependencies 
``` gradle

dependencies {
    compile 'com.sun.easysnackbar:easysnackbar:1.0.1'
    ...
}
```

2. Use in your code
```
 // Must create custom view in this way,so it can display normally
 View contentView = EasySnackBar.convertToContentView(mView, R.layout.layout_custom);
 // true represent show at top,false at bottom
 EasySnackBar.make(mView, contentView, EasySnackBar.LENGTH_SHORT, true).show();
```
