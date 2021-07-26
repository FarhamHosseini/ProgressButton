# ProgressButton
Show or hide Loading on button such as ProgressBar.

## Usage
#### Set up the dependency
1. Add the mavenCentral() repository to your root build.gradle at the end of repositories:
```
allprojects {
	repositories {
		...
		mavenCentral()
	}
}
```
2. Add the ProgressButton dependency in the build.gradle:
```
implementation group: 'com.apachat', name: 'progressbutton-android', version: '1.0.7'
```

Badge:
-----
[![Maven Central](https://img.shields.io/maven-central/v/com.apachat/progressbutton-android.svg?label=Maven%20Central)](https://search.maven.org/search?q=g:%22com.apachat%22%20AND%20a:%22progressbutton-android%22)

## How it works

Sometimes we need to show loading on button as per requirement we don't want to block full screen view with default loading or dialogs. So you can use this library to show loading on button hide loading after that when you want. 

## How to setup

Its very easy to use **ProgressButton** as its a custom button and contain all features of android default button with some extra attributes.

### Add it to a layout

```xml
<layout
     ...
    <com.apachat.progressbutton.core.ProgressButton
            android:id="@+id/progressButton"
            android:layout_width="200dp"
            android:layout_height="51dp"
            android:layout_marginTop="20dp"
            android:paddingLeft="10dp"
            android:paddingRight="10dp"
            android:text="Hello World!"
            android:textColor="@color/white"
            app:lb_buttonColor="@color/colorPrimary"
            app:lb_isShadowEnable="true"
            app:lb_isCircular="true"
            app:lb_loaderColor="@color/colorAccent"
            app:lb_shadowColor="@color/colorPrimaryDark"
            app:lb_shadowHeight="5dp" />
       ...
</layout>
```

### Methods to use in View Class 
   
   You can easily use to show loading on button click by calling `showLoading();` and hide loading by calling 
   `hideLoading();` whenever you want to stop loading.
   
   **Show Loading**
   
   `ProgressButton progressButton = (ProgressButton) findViewById(R.id.progressButton);
    progressButton.showLoading();
   `
   
   **Hide Loading**
    
   `ProgressButton progressButton = (ProgressButton) findViewById(R.id.progressButton);
    progressButton.hideLoading();
    `
