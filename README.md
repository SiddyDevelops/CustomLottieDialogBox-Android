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
## Usage:
In your ```activity.java``` follow the steps given below to add the custom Dialog:
- Step 1. To add an animation from the library-builtin:

	
	CustomLottieDialog customLottieDialog;
	customLottieDialog = new CustomLottieDialog(context, "LO01");
	customLottieDialog.show();
	
- Step 2. To add your own custom <a href="https://lottiefiles.com/">Lottie</a> animation:
	First download Lottie JSON of your preferred animation and add the downloaded file to ``raw`` inside ``res``.
	
![LottiePreview](https://user-images.githubusercontent.com/72121163/135556267-52d16179-3c38-490c-9857-7d5bbbd61c3d.PNG)

	CustomLottieDialog customLottieDialog;
	customLottieDialog = new CustomLottieDialog(context,R.raw.heartbeat_loader);
	customLottieDialog.show();

	
	
	

