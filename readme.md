#Facebook Plugin on Android w/ngCordova
### Using This Project
* `git clone git@github.com:aaronksaunders/ionic-fb-plugin-demo.git`
* `ionic state restore`
* `bower install ngCordova`


### Installing Plugin for Android

Documentation Available Here
* [https://github.com/Telerik-Verified-Plugins/Facebook/blob/master/platforms/android/README.md](https://github.com/Telerik-Verified-Plugins/Facebook/blob/master/platforms/android/README.md)

But also know that in this example I used ngCordova, so see the specific instructions for installing Android, focus on the rebuilding of the project to include the Facebook Libraries
* [http://ngcordova.com/docs/plugins/facebook/](http://ngcordova.com/docs/plugins/facebook/)

This is the actual command I used generate the hash
```
C:\Program Files\Java\jdk1.8.0_31\bin>keytool -exportcert -alias androiddebugkey -keystore %HOMEPATH%\
.android\debug.keystore | openssl sha1 -binary | openssl base64
```
for me it generated this code which i used as the hash in facebook
```
VbivHuwWKSEp9muSx7sP/twxG9s=
```

Install the plugin
```
cordova plugin add https://github.com/Telerik-Verified-Plugins/Facebook --variable APP_ID="1513920088906320" --variable APP_NAME="testfbplugin" 
```
