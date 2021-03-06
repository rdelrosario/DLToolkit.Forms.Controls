## ![](http://res.cloudinary.com/dqeaiomo8/image/upload/c_scale,w_50/v1444578527/DLToolkit/Forms-Controls-128.png) TagEntryView for Xamarin.Forms [![PayPal donate button](http://img.shields.io/paypal/donate.png?color=green)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=VPZ4KHKHXXHR2 "Donate to this project using Paypal") [![Bitcoin donate button](http://img.shields.io/bitcoin/donate.png?color=green)](https://blockchain.info/address/16CvewT3QyAc5ATTVNHQ2EomxLQPXxyKQ7 "Donate to this project using Bitcoin")

Flowing entry with tags/badges support.

NuGet: https://www.nuget.org/packages/DLToolkit.Forms.Controls.TagEntryView/

## Features: 
- Custom bindable tag templates support (any view)
- Custom tag input validator support
- Fully bindable tags
- Configurable minimum entry width
- Flowing layout
- TagTapped event
- All Xamarin.Forms platforms supported

<img src="https://raw.githubusercontent.com/daniel-luberda/DLToolkit.Forms.Controls/master/TagEntryView/Screenshots/Android_01.png" width="250"/> <img src="https://raw.githubusercontent.com/daniel-luberda/DLToolkit.Forms.Controls/master/TagEntryView/Screenshots/Android_02.png" width="250"/>

### Android remarks
Until Xamarin fixes this: [link](http://stackoverflow.com/questions/10593022/monodroid-error-when-calling-constructor-of-custom-view-twodscrollview/10603714#10603714)

You have to add a custom renderer to your Android project to avoid exceptions:

[TagEntryRenderer.cs](https://github.com/daniel-luberda/DLToolkit.Forms.Controls/blob/master/Examples/Droid/Renderers/TagEntryRenderer.cs) 

... and initialize it in `MainActivity.cs`:

`TagEntryRenderer.Init();`

## Demo:

- [TagEntryViewPage.cs](https://github.com/daniel-luberda/DLToolkit.Forms.Controls/blob/master/Examples/Pages/TagEntryViewPage.cs)
- [TagEntryViewViewModel.cs](https://github.com/daniel-luberda/DLToolkit.Forms.Controls/blob/master/Examples/ViewModels/TagEntryViewViewModel.cs)

TIP: Clone repo, open the solution, build it and run sample app. 