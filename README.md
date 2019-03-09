# fb_ssl_pinning

[Facebook V210](https://www.apkmirror.com/apk/facebook-2/facebook/facebook-210-0-0-43-119-release/)

Make sure you have a rooted android device

### steps
* pick your apk here [Facebook](https://www.apkmirror.com/apk/facebook-2/facebook/facebook-210-0-0-43-119-release/facebook-210-0-0-43-119-5-android-apk-download/download/) (check your device via `adb shell getprop ro.product.cpu.abi`)
* open Instagram app on your device, make sure `/data/data/com.facebook.katana/lib-xzs/libcoldstart.so` exists
* download related __.so__ file from current [repo](https://github.com/maoxiao/fb_ssl_pinning)
* run `adb push libcoldstart.so /data/data/com.facebook.katana/lib-xzs/libcoldstart.so`
* setup Burp Suite (please use latest [jdk](https://www.oracle.com/technetwork/java/javase/downloads/jdk11-downloads-5066655.html) to run Burp Suite  `java -jar burpsuite_community.jar`) to intercept requests

