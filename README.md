# RxSwiftFacebook
Facebook Integration With RxSwift.

After creat your project open your project path on terminal and run below mentioned commands for Set up your CocoaPods dependencies

to make a podfile with command:
```
pod init
```
open your podfile with command:
```
open podfile
```
paste pods in your podfile

```
target 'ProjectName' do
  use_frameworks!

   pod 'RxSwift'
   pod 'RxCocoa'
   pod 'FBSDKLoginKit'

end
```
install pod in project with command
```
pod install
```

Login in your Facebook developer Account using https://developers.facebook.com/docs/facebook-login/ios/

Create New App Add Your Bundle identifiers.

After that you get FbId then copy that & provide your application name to for FacebookDisplayName. 

and paste this code in your plist file

```
<key>CFBundleURLTypes</key>
<array>
  <dict>
  <key>CFBundleURLSchemes</key>
  <array>
    <string>Paste our fb Id here</string>
  </array>
  </dict>
</array>
<key>FacebookAppID</key>
<string>Paste our fb Id here</string>
<key>FacebookDisplayName</key>
<string>Your Application Display Name</string>
```
add this for facebook authentication 2.0
```
<key>LSApplicationQueriesSchemes</key>
<array>
  <string>fbapi</string>
  <string>fb-messenger-share-api</string>
  <string>fbauth2</string>
  <string>fbshareextension</string>
</array>
```
Thanks have a nice day.
