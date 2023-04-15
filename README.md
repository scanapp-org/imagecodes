# ImageCodes by ScanApp

A cross platform javascript library for scanning and generating QR codes and barcodes.

This library was forked from [mebjas/html5-qrcode](https://github.com/mebjas/html5-qrcode) by the [mebjas](https://github.com/mebjas) to set path for high quality, performant and scalable library for everyone to scan and generate image codes using javascript.

## Very Important

**Do not use this library yet - it's under development!**
> mebjas@: I have forked and published this package to reserve package name. It's not yet ready for consumption as the APIs are prone to breaking changes in future.

You can follow [this discussion](https://github.com/scanapp-org/imagecodes/discussions/1) to track updates on this library. Meanwhile please continue to use the latest published version of [mebjas/html5-qrcode](https://github.com/mebjas/html5-qrcode).


## Key highlights for the planned library

-   🔲 Support scanning [different types of bar codes and QR codes](#supported-code-formats).

-   🖥 Supports [different platforms](#supported-platforms) be it Android, IOS, MacOs, Windows or Linux

-   🌐 Supports [different browsers](#supported-platforms) like Chrome, Firefox, Safari, Edge, Opera ...

-   📷 Supports scanning with camera as well as local files

-   ➡️ Comes with an [end to end library with UI](#easy-mode---with-end-to-end-scanner-user-interface) as well as a [low level library to build your own UI with](#pro-mode---if-you-want-to-implement-your-own-user-interface).

-   🔦 Supports customisations like [flash/torch support](#showtorchbuttonifsupported---boolean--undefined), zooming etc.

-   Supports scanning as well as generating image codes.

## We need your help!

![image](https://user-images.githubusercontent.com/3007365/222830114-e5bcca15-bf8a-434e-9f48-339e82a0a4ef.png)
Help incentivise feature development, bug fixing by supporting the sponsorhip goals of this project. See [list of sponsered feature requests here](https://github.com/mebjas/html5-qrcode/wiki/Feature-request-sponsorship-goals#feature-requests).

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/L3L84G0C8)

## Supported platforms

We are working continuously on adding support for more and more platforms. If you find a platform or a browser where the library is not working, please feel free to file an issue. Check the [demo link](https://blog.minhazav.dev/research/html5-qrcode.html) to test it out.

**Legends**
-   ![](https://scanapp.org/assets/github_assets/done.png) Means full support — inline webcam and file based 
-   ![](https://scanapp.org/assets/github_assets/partial.png) Means partial support — only file based, webcam in progress

### PC / Mac

| <img src="https://scanapp.org/assets/github_assets/browsers/firefox_48x48.png" alt="Firefox" width="24px" height="24px" /><br/>Firefox | <img src="https://scanapp.org/assets/github_assets/browsers/chrome_48x48.png" alt="Chrome" width="24px" height="24px" /><br/>Chrome | <img src="https://scanapp.org/assets/github_assets/browsers/safari_48x48.png" alt="Safari" width="24px" height="24px" /><br/>Safari | <img src="https://scanapp.org/assets/github_assets/browsers/opera_48x48.png" alt="Opera" width="24px" height="24px" /><br/>Opera | <img src="https://scanapp.org/assets/github_assets/browsers/edge_48x48.png" alt="Edge" width="24px" height="24px" /><br/> Edge
| --------- | --------- | --------- | --------- | ------- |
|![](https://scanapp.org/assets/github_assets/done.png)| ![](https://scanapp.org/assets/github_assets/done.png)| ![](https://scanapp.org/assets/github_assets/done.png)| ![](https://scanapp.org/assets/github_assets/done.png) | ![](https://scanapp.org/assets/github_assets/done.png)

### Android

| <img src="https://scanapp.org/assets/github_assets/browsers/chrome_48x48.png" alt="Chrome" width="24px" height="24px" /><br/>Chrome | <img src="https://scanapp.org/assets/github_assets/browsers/firefox_48x48.png" alt="Firefox" width="24px" height="24px" /><br/>Firefox | <img src="https://scanapp.org/assets/github_assets/browsers/edge_48x48.png" alt="Edge" width="24px" height="24px" /><br/> Edge | <img src="https://scanapp.org/assets/github_assets/browsers/opera_48x48.png" alt="Opera" width="24px" height="24px" /><br/>Opera | <img src="https://scanapp.org/assets/github_assets/browsers/opera-mini_48x48.png" alt="Opera-Mini" width="24px" height="24px" /><br/> Opera Mini | <img src="https://scanapp.org/assets/github_assets/browsers/uc_48x48.png" alt="UC" width="24px" height="24px" /> <br/> UC
| --------- | --------- | --------- | --------- |  --------- | --------- |
|![](https://scanapp.org/assets/github_assets/done.png)| ![](https://scanapp.org/assets/github_assets/done.png)| ![](https://scanapp.org/assets/github_assets/done.png)| ![](https://scanapp.org/assets/github_assets/done.png)| ![](https://scanapp.org/assets/github_assets/partial.png) | ![](https://scanapp.org/assets/github_assets/partial.png) 

### IOS

| <img src="https://scanapp.org/assets/github_assets/browsers/safari_48x48.png" alt="Safari" width="24px" height="24px" /><br/>Safari | <img src="https://scanapp.org/assets/github_assets/browsers/chrome_48x48.png" alt="Chrome" width="24px" height="24px" /><br/>Chrome | <img src="https://scanapp.org/assets/github_assets/browsers/firefox_48x48.png" alt="Firefox" width="24px" height="24px" /><br/>Firefox | <img src="https://scanapp.org/assets/github_assets/browsers/edge_48x48.png" alt="Edge" width="24px" height="24px" /><br/> Edge 
| --------- | --------- | --------- | --------- |
|![](https://scanapp.org/assets/github_assets/done.png)| ![](https://scanapp.org/assets/github_assets/done.png)* | ![](https://scanapp.org/assets/github_assets/done.png)* | ![](https://scanapp.org/assets/github_assets/partial.png) 


> \* Supported for IOS versions >= 15.1
>
> Before version 15.1, Webkit for IOS is used by Chrome, Firefox, and other browsers in IOS and they do not have webcam permissions yet. There is an ongoing issue on fixing the support for iOS - [issue/14](https://github.com/mebjas/html5-qrcode/issues/14)

### Framework support
The library can be easily used with several other frameworks, I have been adding examples for a few of them and would continue to add more.

|<img src="https://scanapp.org/assets/github_assets/html5.png" width="30px" />| <img src="https://scanapp.org/assets/github_assets/vuejs.png" width="30px" />|<img src="https://scanapp.org/assets/github_assets/electron.png" width="30px" /> | <img src="https://scanapp.org/assets/github_assets/react.svg" width="30px" /> | <img src="https://seeklogo.com/images/L/lit-logo-6B43868CDC-seeklogo.com.png" width="30px" />
| -------- | -------- | -------- | -------- | -------- |
| [Html5](./examples/html5) | [VueJs](./examples/vuejs) | [ElectronJs](./examples/electron) | [React](https://github.com/scanapp-org/html5-qrcode-react) | [Lit](./examples/lit)

### Supported Code formats
Code scanning is dependent on [Zxing-js](https://github.com/zxing-js/library) library. We will be working on top of it to add support for more types of code scanning. If you feel a certain type of code would be helpful to have, please file a feature request.

| Code | Example |
| ---- | ----- |
| QR Code | <img src="https://scanapp.org/assets/github_assets/qr-code.png" width="200px" /> |
| AZTEC | <img src="https://scanapp.org/assets/github_assets/aztec.png" /> |
| CODE_39|  <img src="https://scanapp.org/assets/github_assets/code_39.gif" /> |
| CODE_93| <img src="https://scanapp.org/assets/github_assets/code_93.gif" />|
| CODE_128| <img src="https://scanapp.org/assets/github_assets/code_128.gif" />|
| ITF| <img src="https://scanapp.org/assets/github_assets/itf.png" />|
| EAN_13|<img src="https://scanapp.org/assets/github_assets/ean13.jpeg" /> |
| EAN_8| <img src="https://scanapp.org/assets/github_assets/ean8.jpeg" />|
| PDF_417| <img src="https://scanapp.org/assets/github_assets/pdf417.png" />|
| UPC_A| <img src="https://scanapp.org/assets/github_assets/upca.jpeg" />|
| UPC_E| <img src="https://scanapp.org/assets/github_assets/upce.jpeg" />|
| DATA_MATRIX|<img src="https://scanapp.org/assets/github_assets/datamatrix.png" /> |
| MAXICODE*| <img src="https://scanapp.org/assets/github_assets/maxicode.gif" /> |
| RSS_14*| <img src="https://scanapp.org/assets/github_assets/rss14.gif" />|
| RSS_EXPANDED*|<img src="https://scanapp.org/assets/github_assets/rssexpanded.gif" /> |

> *Formats are not supported by our experimental integration with native
> BarcodeDetector API integration ([Read more](/experimental.md)).

## Support 💖

This project would not be possible without all of our fantastic contributors and [sponsors](https://github.com/sponsors/mebjas). If you'd like to support the maintenance and upkeep of this project you can [donate via GitHub Sponsors](https://github.com/sponsors/mebjas).

**Sponsor the project for priortising feature requests / bugs relevant to you**. (Depends on scope of ask and bandwidth of the contributors).

<!-- sponsors -->
<a href="https://github.com/webauthor"><img src="https://github.com/webauthor.png" width="40px" alt="webauthor@" /></a>
<a href="https://github.com/ben-gy"><img src="https://github.com/ben-gy.png" width="40px" alt="ben-gy" /></a>
<a href="https://github.com/bujjivadu"><img src="https://github.com/bujjivadu.png" width="40px" alt="bujjivadu" /></a>
<!-- sponsors -->

Help incentivise feature development, bug fixing by supporting the sponsorhip goals of this project. See [list of sponsered feature requests here](https://github.com/mebjas/html5-qrcode/wiki/Feature-request-sponsorship-goals#feature-requests).

Also, huge thanks to following organizations for non monitery sponsorships

<!-- sponsors -->
<div>
	<a href="https://scanapp.org"><img src="https://scanapp.org/assets/svg/scanapp.svg" height="60px" alt="" /></a>
</div>
<div>
	<a href="https://www.browserstack.com"><img src="https://www.browserstack.com/images/layout/browserstack-logo-600x315.png" height="100px" alt="" /></a>
</div>
<!-- sponsors -->

## Credits
The decoder used for the QR code reading is from `Zxing-js` https://github.com/zxing-js/library<br />
