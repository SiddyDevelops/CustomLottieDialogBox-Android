# CustomLottieDialogBox
<img align="right" alt="Coding" width="300" height="300" src="https://user-images.githubusercontent.com/72121163/135441308-2fd004ca-caaf-4b7f-b760-a29c5aecbe46.gif">

## About
CustomLottieDialogBox is an android library which facilitate developers to add customized loading Dialog-Boxes to their android apps. Users can add Lottie Animations of thier wish or can choose from the already existing animation. They can change the backgroung color, text color, size of dialog box or can add thier own custom text using this library.

[![](https://jitpack.io/v/SiddyDevelops/CustomLottieDialogBox-Android.svg)](https://jitpack.io/#SiddyDevelops/CustomLottieDialogBox-Android)
![Minimum SDK Version](https://img.shields.io/badge/minSdkVersion-23-brightgreen)
[![Platform](https://img.shields.io/badge/platform-android-green.svg)](http://developer.android.com/index.html)

<p align="center">
  <img width="150" height="350" src="https://user-images.githubusercontent.com/72121163/135487978-925d83ef-6745-4b34-8081-6d916083293d.gif">  
  <img width="150" height="350" src="https://user-images.githubusercontent.com/72121163/135488088-67315429-f074-4f3c-8735-017e85baa634.gif">
  <img width="150" height="350" src="https://user-images.githubusercontent.com/72121163/135488105-abbbf44b-bfd7-4cfb-ab2f-a1bd18af5d42.gif">
</p>

---

## Installation:
- Step 1. Add it in your root build.gradle at the end of repositories:
```
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
- Step 2. Add the dependency:
```
dependencies {
	        implementation 'com.github.SiddyDevelops:CustomLottieDialogBox-Android:0.2.0'
	}
```

---

## Usage:
In your ```activity.java``` follow the steps given below to add the custom Dialog:
- To add an animation from the library-builtin:

 	```
	CustomLottieDialog customLottieDialog;
	customLottieDialog = new CustomLottieDialog(context, "LO01");
	customLottieDialog.show();
	```
	Kotlin Code 
	```
	val customLottieDialog: CustomLottieDialog
        customLottieDialog = CustomLottieDialog(this, "LO01")
        customLottieDialog.show()
	```
	
- To add your own custom <a href="https://lottiefiles.com/">Lottie</a> animation:  First download Lottie JSON of your preferred animation and add the downloaded file to ``raw`` inside ``res``.
	
![LottiePreview](https://user-images.githubusercontent.com/72121163/135556267-52d16179-3c38-490c-9857-7d5bbbd61c3d.PNG)

	CustomLottieDialog customLottieDialog;
	customLottieDialog = new CustomLottieDialog(context,R.raw.heartbeat_loader);
	customLottieDialog.show();

- To customize the Loading Text:

	```
	customLottieDialog.setLoadingText("Custom Text");
			OR
	customLottieDialog.setLoadingText("");          //-----> To remove custom text
	```
- To change text-color of custom loading text:
	
	```
	customLottieDialog.setLoadingTextColor("{HexColorCode}");
	```

- To change Lottie animation background color:
	```
	customLottieDialog.setLottieBackgroundColor("{HexColorCode}");
	```
	
- To change the dimensions of the dialog box:
	
	```
	customLottieDialog.setDialogLayoutDimensions({width in dp (int)},{height in dp (int));
	```

- To dismiss the dialog box:
	
	```
	customLottieDialog.dismiss();
	```

- Example:
	
	```
	CustomLottieDialog customLottieDialog;
	customLottieDialog = new CustomLottieDialog(MainActivity.this, "LO01");
	customLottieDialog.setLottieBackgroundColor("#7AC89E");
	customLottieDialog.setLoadingText("Custom Text");
	customLottieDialog.setLoadingTextColor("#FFFFFF");
	```
	
---

## Library-Inbuilt Animations:

<table>
<tr><th></th><th></th></tr>
<tr><td>

| Animation | lottieBatch | 
|--|--|
| <img src='https://user-images.githubusercontent.com/72121163/135574362-f374c0f6-f9cb-43d5-84b4-34b80ca657f6.gif' alt='PaperPlane' width="150px" height="150px"/> | "LO01" |
| <img src='https://user-images.githubusercontent.com/72121163/135576133-7305c74f-8782-4e55-b1bf-4cb0462eaba6.gif' alt='Balance' width="150px" height="150px"/> | "LO03" |
| <img src='https://user-images.githubusercontent.com/72121163/135577221-740d5817-a54e-48cc-909b-e586dd4179e7.gif' alt='Loop' width="150px" height="150px"/> | "LO05" |
| <img src='https://user-images.githubusercontent.com/72121163/135577712-bfd3e3c5-9365-41db-949d-44567ee303da.gif' alt='Rocket' width="150px" height="150px"/> | "LO07" |

</td><td>

| Animation | lottieBatch |
|--|--|
| <img src='https://user-images.githubusercontent.com/72121163/135574595-4cd8b4bc-3b36-4057-af55-1cfe08db7755.gif' alt='Bubble' width="150px" height="150px"/> | "LO02" |
| <img src='https://user-images.githubusercontent.com/72121163/135576343-aab0053b-5265-4965-899a-e81e19c0aa4f.gif' alt='Groove' width="150px" height="150px"/> | "LO04" |
| <img src='https://user-images.githubusercontent.com/72121163/135577352-8acb9019-15a4-4bd0-b57f-b4ab988ff1a4.gif' alt='Music' width="150px" height="150px"/> | "LO06" |
| <img src='https://user-images.githubusercontent.com/72121163/135577931-b2a8e22b-05ed-4673-a816-e611a197dd54.gif' alt='Spiral' width="150px" height="150px"/> | "LO08" |

</td></tr> 
</table>
	
---
	
## From the Developer:

This Android Library is developed by <a href="https://github.com/SiddyDevelops">Siddharth Singh<a/>. The animation included in this library is taken from https://lottiefiles.com/ .
  
Follow my <a href="https://github.com/SiddyDevelops#connect-with-me">Social Handles<a/> for more projects.
  
Enjoy Coding!! 🚀 ✨

---





