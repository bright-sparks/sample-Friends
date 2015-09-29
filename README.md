
# Telerik Friends Sample App for NativeScript

<a href="https://platform.telerik.com/#appbuilder/clone/https://github.com/NativeScript/sample-Friends/" target="_blank"><img src="http://docs.telerik.com/platform/appbuilder/sample-apps/images/try-in-appbuilder.png" alt="Try in AppBuilder" title="Try in Telerik Platform" /></a> <a href="https://github.com/NativeScript/sample-Friends/" target="_blank"><img style="padding-left:20px" src="http://docs.telerik.com/platform/appbuilder/sample-apps/images/get-github.png" alt="Get from GitHub" title="Get from GitHub"></a>

* [Overview](#overview)
* [Requirements](#requirements)
* [Configuration](#configuration)
* [Running the Sample](#running-the-sample)

## Overview

This repository contains the Telerik Friends app for PhoneGap/Cordova. It is a sample mobile app demonstrating how to integrate a large gamut of Telerik Platform services into a native mobile application using the [NativeScript](http://github.com/nativescript/nativescript) framework.

The Telerik Friends sample app showcases these features and SDKs:

- Cloud data access (Telerik Backend Services)
- Working with files (Telerik Backend Services)
- User registration and authentication (Telerik Backend Services)
- Using custom user account fields (Telerik Backend Services)
- Basic app analytics (Telerik Analytics)
- Tracking feature usage (Telerik Analytics)

- Authentication with social login providers (Facebook, Google, etc.) (Telerik Backend Services)
- Authentication with AD FS (Telerik Backend Services)

To implement all the features listed above, the sample app utilizes the following Telerik products and SDKs:

- Telerik Backend Services - this is where all data, files, and user accounts are stored in the cloud
- Telerik Backend Services JavaScript SDK - to connect the app to Telerik Backend Services
- Telerik Analytics - used to store and monitor analytics data in the cloud
- Telerik Analytics JavaScript SDK - to connect the app with Telerik Analytics


## Requirements

Before you begin, you need to ensure that you have the following:

- **An active Telerik Platform account**
Ensure that you can log in to a Telerik Platform account. This can be a free trial account. Depending on your license you may not be able to use all app features. For more information on what is included in the different editions, check out the pricing page. All features included in the sample app work during the free trial period.

- **Telerik AppBuilder** The sample app requires Telerik AppBuilder to run. This can be the in-browser client, the desktop client or the extension for Visual Studio.

## Configuration

The Friends sample app comes fully functional, but to see it in action you must link it to your own Telerik Platform account.

1. Click the "Try in AppBuilder" button to clone the repository in AppBuilder.<br>
	An app called "My App" is created for you with an AppBuilder project set up.
2. Click **My App** in the navigation bar at the top to go the app home.
3. Create a Backend Services project, selecting the **Start from the Friends app** option.
4. Once the Backend Services project is ready, go to **Overview > API Keys**.
5. Take note of your API Key.
6. Go back to the AppBuilder project and continue setting up as explained in the next sections.

### API Key for Telerik Backend Services

This is a unique string that links the sample mobile app to a project in Telerik Backend Services where all the data is read from/saved. When creating the project, you must base it on the Friends sample Backend Services project that has all the necessary data prepopulated.

You must use this project's API key. To set it in the app:

1. Open the `/app/app.js` file.
2. Replace `$EVERLIVE_API_KEY$` with the API Key of your Friends Backend Services project.

> If you happen to break the structure of the automatically generated Friends sample project, you can delete it and a fresh instance will be created again for you automatically. Alternatively, you could create a new project and choose to start from a Friends template, instead of starting from a blank project.

### (Optional) Project Key for Telerik Analytics

This is a unique string that links the sample mobile app to a Telerik Analytics project in your account. If you do not set this the sample will still work, but no analytics data will be collected.
	
1. Open the `/app/views/main-page.js` file.
2. Replace `$EQATEC_PROJECT_KEY$` with the Project Key of your Friends Analytics project.

### HTTPS Connections

By default the Friends Sample is configured to use HTTP. If you want to switch to HTTPS, update the `global.BS_SCHEME` setting in  `/app/app.js` to `https`.

## Running the Sample

Once the app is configured, you can run it either on a real device or a native emulator.

To run it, follow the steps in the product's documentation: [Running Apps on Devices](http://docs.telerik.com/platform/appbuilder/testing-your-app/running-on-devices/working-with-devices).

> Ensure that the emulator or the device that you are using has Internet connectivity when running the sample.









 