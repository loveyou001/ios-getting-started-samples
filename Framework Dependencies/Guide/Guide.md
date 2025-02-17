# Framework Dependencies

In the Creative SDK for iOS, we've broken the Foundation framework into Micro frameworks so that developers can include only the pieces that they need, thereby reducing the size of their binary. The AdobeCreativeSDKFoundation framework has been divided into the following frameworks:

- AdobeCreativeSDKCore
- AdobeCreativeSDKCommonUX
- AdobeCreativeSDKAppLibraryUX
- AdobeCreativeSDKAssetModel
- AdobeCreativeSDKAssetUX
- AdobeCreativeSDKMarketUX

You can read more about the Framework breakup on our <a target="_blank" href="https://blog.creativesdk.com/2015/08/dividing-up-the-foundation-sdk/">blog</a>.

## Migrating from Monolithic Foundation Framework to Framework Breakup (v0.11.2118+)

When migrating from the old Foundation Framework to the newer Creative SDK, you'll need to update previous references to `AdobeCreativeSDKFoundation/AdobeCreativeSDKFoundation.h` with the new broken up header file(s). See below for a full list.

## Frameworks Overview

Below is a table that contains all of the Framework and header dependencies for each feature of the Creative SDK:

<table>
   <tbody>
      <tr>
         <th colspan="1">Feature</th>
         <th colspan="1">Framework</th>
         <th>Framework/Headers</th>
      </tr>
      <tr>
         <td colspan="1">Authentication</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
         </td>
         <td colspan="1">
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
         </td>
      </tr>
      <tr>
         <td colspan="1">Asset Browser UI Component</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#commonux">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>
            <br /><a href="#assetux">AdobeCreativeSDKAssetUX.framework</a>
         </td>
         <td colspan="1">
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
            <br />AdobeCreativeSDKAssetUX/AdobeCreativeSDKAssetUX.h
         </td>
      </tr>
      <tr>
         <td colspan="1">Lightroom Upload UI Component</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#commonux">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>
            <br /><a href="#assetux">AdobeCreativeSDKAssetUX.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
            <br />AdobeCreativeSDKAssetUX/AdobeCreativeSDKAssetUX.h
         </td>
      </tr>
      <tr>
         <td colspan="1">Creative Cloud Files API</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#commonux">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>
            <br /><a href="#assetux">AdobeCreativeSDKAssetUX.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
            <br />AdobeCreativeSDKAssetUX/AdobeCreativeSDKAssetUX.h
         </td>
      </tr>
      <tr>
         <td colspan="1">Lightroom Photos API</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#commonux">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>
            <br /><a href="#assetux">AdobeCreativeSDKAssetUX.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
            <br />AdobeCreativeSDKAssetUX/AdobeCreativeSDKAssetUX.h
         </td>
      </tr>
      <tr>
         <td colspan="1">Creative Cloud Libraries</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>

            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>

         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
         </td>
      </tr>
      <tr>
         <td>Creative Cloud Market UI Component</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#commonux">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>
            <br /><a href="#assetux">AdobeCreativeSDKAssetUX.framework</a>
            <br /><a href="#marketux">AdobeCreativeSDKMarketUX.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
            <br />AdobeCreativeSDKAssetUX/AdobeCreativeSDKAssetUX.h
            <br />AdobeCreativeSDKMarketUX/AdobeCreativeSDKMarketUX.h
         </td>
      </tr>
      <tr>
         <td>Image Editor UI Component</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>

            <br /><a href="#imageeditor">AdobeCreativeSDKImage.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKImage/AdobeCreativeSDKImage.h
         </td>
      </tr>
      <tr>
         <td>Color Tool UI Component</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#commonux">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>
            <br /><a href="#assetux">AdobeCreativeSDKAssetUX.framework</a>
            <br /><a href="#colorcomponent">AdobeCreativeSDKColorComponent.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
            <br />AdobeCreativeSDKAssetUX/AdobeCreativeSDKAssetUX.h
            <br />AdobeCreativeSDKColorComponent/AdobeCreativeSDKColorComponent.h
         </td>
      </tr>
      <tr>
         <td>Share Menu UI Component</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#commonux">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>
            <br /><a href="#assetux">AdobeCreativeSDKAssetUX.framework</a>
            <br /><a href="#behance">AdobeCreativeSDKBehance.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
            <br />AdobeCreativeSDKAssetUX/AdobeCreativeSDKAssetUX.h
            <br />AdobeCreativeSDKBehance/AdobePublishShareMenu.h
         </td>
      </tr>
      <tr>
         <td>SendToDesktop API</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>

            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>

         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
         </td>
      </tr>
      <tr>
         <td>Application Library UI Component</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#commonux">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#applibraryux">AdobeCreativeSDKAppLibraryUX.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAppLibraryUX/AdobeCreativeSDKAppLibraryUX.h
         </td>
      </tr>
      <tr>
         <td>Behance UI Component</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>
            <br /><a href="#core">AdobeCreativeSDKCommonUX.framework</a>
            <br /><a href="#assetmodel">AdobeCreativeSDKAssetModel.framework</a>
            <br /><a href="#assetux">AdobeCreativeSDKAssetUX.framework</a>
            <br /><a href="#behance">AdobeCreativeSDKBehance.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKCommonUX/AdobeCreativeSDKCommonUX.h
            <br />AdobeCreativeSDKAssetModel/AdobeCreativeSDKAssetModel.h
            <br />AdobeCreativeSDKAssetUX/AdobeCreativeSDKAssetUX.h
            <br />AdobeCreativeSDKBehance/AdobePublish.h
         </td>
      </tr>
      <tr>
         <td>Magic Selection View UI</td>
         <td colspan="1">
            <a href="#core">AdobeCreativeSDKCore.framework</a>

            <br /><a href="#labs">AdobeCreativeSDKLabs.framework</a>
         </td>
         <td>
            AdobeCreativeSDKCore/AdobeCreativeSDKCore.h
            <br />AdobeCreativeSDKLabs/AdobeCreativeSDKLabs.h
         </td>
      </tr>
   </tbody>
</table>


## Individual Frameworks

The following section outlines the required setup for each part of the Creative SDK.

### Frameworks

+ [AdobeCreativeSDKCore](#core)
+ [AdobeCreativeSDKCommonUX](#commonux)
+ [AdobeCreativeSDKAppLibraryUX](#applibraryux)
+ [AdobeCreativeSDKAssetModel](#assetmodel)
+ [AdobeCreativeSDKAssetUX](#assetux)
+ [AdobeCreativeSDKMarketUX](#marketux)
+ [AdobeCreativeSDKColorComponent](#colorcomponent)
+ [AdobeCreativeSDKDevice](#device)
+ [AdobeCreativeSDKImage](#imageeditor)
+ [AdobeCreativeSDKBehance](#behance)
+ [AdobeCreativeSDKLabs](#labs)


<a name="core"></a>
### AdobeCreativeSDKCore

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select AdobeCreativeSDKCore.bundle. This file may be found where you extracted the SDK at AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle.
3. In Build Phases, Link Binary with Libraries, add the AdobeCreativeSDKCore.framework folder.
4. In the same area, add the following libraries:
    + MobileCoreServices.framework
    + SystemConfiguration.framework
    + libc++.dylib
    + libz.dylib
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="commonux"></a>
### AdobeCreativeSDKCommonUX

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKCommonUX.framework/Resources/AdobeCreativeSDKCommonUXResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKCommonUX.framework
4. In the same area, add the following libraries:
    + MobileCoreServices.framework
    + SystemConfiguration.framework
    + libc++.dylib
    + libz.dylib
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="applibraryux"></a>
### AdobeCreativeSDKAppLibraryUX

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKCommonUX.framework/Resources/AdobeCreativeSDKCommonUXResources.bundle
    + AdobeCreativeSDKAssetModel.framework/Resources/AdobeCreativeSDKAssetModelResources.bundle
    + AdobeCreativeSDKAppLibraryUX.framework/Resources/AdobeCreativeSDKAppLibraryUXResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKCommonUX.framework
    + AdobeCreativeSDKAssetModel.framework
    + AdobeCreativeSDKAppLibraryUX.framework
4. In the same area, add the following libraries:
    + MobileCoreServices.framework
    + SystemConfiguration.framework
    + libc++.dylib
    + libz.dylib
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="assetmodel"></a>
### AdobeCreativeSDKAssetModel

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKAssetModel.framework/Resources/AdobeCreativeSDKAssetModelResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKAssetModel.framework
4. In the same area, add the following libraries:
    + MobileCoreServices.framework
    + SystemConfiguration.framework
    + libc++.dylib
    + libz.dylib
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="assetux"></a>
### AdobeCreativeSDKAssetUX

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKCommonUX.framework/Resources/AdobeCreativeSDKCommonUXResources.bundle
    + AdobeCreativeSDKAssetModel.framework/Resources/AdobeCreativeSDKAssetModelResources.bundle
    + AdobeCreativeSDKAssetUX.framework/Resources/AdobeCreativeSDKAssetUXResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKAssetModel.framework
    + AdobeCreativeSDKAssetUX.framework
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKCommonUX.framework
4. In the same area, add the following libraries:
    + MobileCoreServices.framework
    + SystemConfiguration.framework
    + libc++.dylib
    + libz.dylib
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="marketux"></a>
### AdobeCreativeSDKMarketUX

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKCommonUX.framework/Resources/AdobeCreativeSDKCommonUXResources.bundle
    + AdobeCreativeSDKAssetModel.framework/Resources/AdobeCreativeSDKAssetModelResources.bundle
    + AdobeCreativeSDKAssetUX.framework/Resources/AdobeCreativeSDKAssetUXResources.bundle
    + AdobeCreativeSDKMarketUX.framework/Resources/AdobeCreativeSDKMarketUXResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKAssetModel.framework
    + AdobeCreativeSDKAssetUX.framework
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKCommonUX.framework
    + AdobeCreativeSDKMarketUX.framework
4. In the same area, add the following libraries:
    + MobileCoreServices.framework
    + SystemConfiguration.framework
    + libc++.dylib
    + libz.dylib
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="colorcomponent"></a>
### AdobeCreativeSDKColorComponent

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKAssetModel.framework/Resources/AdobeCreativeSDKAssetModelResources.bundle
    + AdobeCreativeSDKColorComponent.framework/Resources/AdobeCreativeSDKColorComponenentResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKAssetModel.framework
    + AdobeCreativeSDKColorComponent.framework
5. In the same area, add the following libraries:
    + MobileCoreServices.framework
    + SystemConfiguration.framework
    + libc++.dylib
    + libz.dylib
6. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="device"></a>
### AdobeCreativeSDKDevice

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKAssetModel.framework/Resources/AdobeCreativeSDKAssetModelResources.bundle
    + AdobeCreativeSDKColorComponent.framework/Resources/AdobeCreativeSDKColorComponenentResources.bundle
    + AdobeCreativeSDKDevice.framework/Resources/AdobeCreativeSDKDeviceResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following libraries:
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKAssetModel.framework 
    + AdobeCreativeSDKColorComponent.framework
    + AdobeCreativeSDKDevice.framework
    + Ink Support:
        * AdobeCreativeSDKDeviceExtensionJotTouchSDK.framework
        * JotTouchSDK.framework
    + Wacom Support:
        * AdobeCreativeSDKDeviceExtensionWacomDevice.framework
        * The WacomDevice.framework available from Wacom's iOS Developer <a href="http://www.wacom.com/en-us/enterprise/business-solutions/software-and-solutions/sdks" target="_blank">site</a>.
    + Pencil 53 Support:
        + AdobeCreativeSDKDeviceExtensionFiftyThreeSdk.framework
        + The FiftyThreeSdk.framework available from Pencil 53’s iOS Developer <a href="http://www.fiftythree.com/pencil" target="_blank">site</a>.
4. In the same area, add the following libraries:
    + libc++.dylib
    + libz.dylib
    + CoreBluetooth.framework
    + CoreMotion.framework
    + MobileCoreServices.framework
    + SystemConfiguration.framework
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="imageeditor"></a>
### AdobeCreativeSDKImage

The following configuration settings are required for this framework:

1. Add -ObjC and -all_load as linker flags in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKImage.framework/Resources/AdobeCreativeSDKImageResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKImage.framework
4. In the same area, add the following libraries:
    + Accelerate.framework
    + CoreData.framework
    + libsqlite3.0.dylib
    + libz.1.2.5.dylib
    + Foundation.framework
    + MessageUI.framework
    + OpenGLES.framework
    + QuartzCore.framework
    + StoreKit.framework
    + UIKit.framework
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="behance"></a>
### AdobeCreativeSDKBehance

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKCommonUX.framework/Resources/AdobeCreativeSDKCommonUXResources.bundle
    + AdobeCreativeSDKAssetModel.framework/Resources/AdobeCreativeSDKAssetModelResources.bundle
    + AdobeCreativeSDKAssetUX.framework/Resources/AdobeCreativeSDKAssetUXResources.bundle
    + AdobeCreativeSDKBehance.framework/Resources/AdobeCreativeSDKBehanceResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKAssetModel.framework
    + AdobeCreativeSDKAssetUX.framework
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKCommonUX.framework
    + AdobeCreativeSDKBehance.framework
4. In the same area, add the following libraries:
    + libc++.dylib
    + libz.dylib
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.

<a name="labs"></a>
### AdobeCreativeSDKLabs

The following configuration settings are required for this framework:

1. Add -ObjC as a linker flag in Build Settings/Linking/Other Linker Flags.
2. In Build Phases, expand Copy Bundle Resources, click the + button, select "Add Other" and select the following bundles:
    + AdobeCreativeSDKCore.framework/Resources/AdobeCreativeSDKCoreResources.bundle
    + AdobeCreativeSDKLabs.framework/Resources/AdobeCreativeSDKLabsResources.bundle
3. In Build Phases, Link Binary with Libraries, add the following:
    + AdobeCreativeSDKCore.framework
    + AdobeCreativeSDKLabs.framework
4. In the same area, add the following libraries:
    + MobileCoreServices.framework
    + SystemConfiguration.framework
    + libc++.dylib
    + libz.dylib
5. In Build Settings, Apple LLVM 6.1 - Preprocessing, add *USE_CSDK_COMPONENTS* to the *Preprocessor Macros*.