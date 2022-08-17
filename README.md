# Veriff Library Binding For Xamarin IOS 

Veriff Library IOS Latest Version v4.42.0 Bindings For Xamarin IOS Dll Files Are given in repository.</br> 
You can use any Veriff function in your xamarin ios porject by referencing the dll file in your project.
</br>
<b>Please Note:</b>

For Running Xamarin IOS Project on Your Simulator You Have To Reference <b>"VeriffIOSLibrary.dll"</b> in Your Project.</br>
For Running Xamarin IOS Project on Your Physical Device You Have To Reference <b>"VeriffReleaseLibraryIOS.dll"</b> in Your Project.</br>

</br>
You Can use below provided documentation in order to consume Veriff Functions.
</br>
<b>Official Documentation Link For Integrating Veriff In Your IOS Project:</b>
https://developers.veriff.com/#ios-sdk-integration

</br>


</br>
<a href="https://www.buymeacoffee.com/faisaltanvC" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
</br></br>

<b>Add usage descriptions to application Info.plist</b>

    Not adding these usage descriptions causes system to kill application when it requests the permissions when needed.

<b>Veriff iOS SDK requires Following Permissions:</b>

    NSCameraUsageDescription
    NSMicrophoneUsageDescription
    NSPhotoLibraryUsageDescription
    NFCReaderUsageDescription

<b>Add required steps for NFC scanning</b>

The application needs to define the list of application IDs or AIDs it can connect to, in the Info.plist file. The AID is a way of uniquely identifying an application on a ISO 7816 tag, which is usually defined by a standard.

<key>com.apple.developer.nfc.readersession.iso7816.select-identifiers</key>
<array>
  <string>A0000002471001</string>
  <string>A0000002472001</string>
  <string>00000000000000</string>
</array>

Add a new entitlement for NFC scanning, available since iOS 13. This new entitlement is added automatically by Xcode when enabling the Near Field Communication Tag Reading capability in the target Signing & Capabilities. After enabling the capability the *.entitlements file needs to contain the TAG format:

<key>com.apple.developer.nfc.readersession.formats</key>
<array>
    <string>NDEF</string>
    <string>TAG</string>
</array>


</br></br></br>
<b>Veriff IOS SDK DLL Bindings</b><br>
<b>veriff integration</b>
