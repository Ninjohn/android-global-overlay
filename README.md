# GlobalOverlayService #

I went through about 10 other implementations of the global floating overlays and none of them were as modular as I would have liked. So, this is my implementation.



## Features ##

1. Easy, readable implementation
2. Overlay view dragging
3. Simple onClick and onRemove listeners
4. Close view by dragging to an "X" view at the bottom of the screen



## Usage ##

1. Set this project as a dependency.
2. Subclass `GlobalOverlayService`. Add your subclass to `AndroidManifest.xml`. Also, add the permission `<uses-permission android:name="android.permission.SYSTEM_ALERT_WINDOW"/>`.
3. Call `addOverlayView(View)`

Done. Most cases won't need to do any more than that. Though there are a few more methods to support other use cases.

`GlobalOverlayService` will handle everything else, including closing the overlay view when the `Service` is destroyed.



## Contributing ##

Have fun.

[AOSP code style](https://source.android.com/source/code-style.html) preferred.



## License ##
MIT