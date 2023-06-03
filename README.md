## Repo For Ionic Bug

bug: ion-title is covered when text of ion-back-button is too long

## Current Behavior

ion-title is covered when text of ion-back-button is too long.

![image](https://github.com/ionic-team/ionic-framework/assets/20255750/b62ef4ad-453c-4857-9888-12d99eb3752b)

## Expected Behavior

When the text of the back button is too long, hide the excess and trailing `...`, just like the title does for long text.

![image](https://github.com/ionic-team/ionic-framework/assets/20255750/3a00b884-c412-4095-af4e-1211146d646d)

It looks like this:

![image](https://github.com/ionic-team/ionic-framework/assets/20255750/e0da75c9-6c23-4910-b1ee-ba6d0ea8b509)

## Steps to Reproduce

1. Run `git clone https://github.com/angelofan/ion-back-button-text.git`
2. Run `npm install`
3. Run to Web.
4. Click the `Go to new page` button.
5. Swipe up in the new page, and the text of the back button covers the title.

## Ionic Info

```
[WARN] Error loading @ionic/angular package.json: Error [ERR_PACKAGE_PATH_NOT_EXPORTED]: Package subpath './package' is
       not defined by "exports" in D:\myrepo\ion-back-button-text\node_modules\@ionic\angular\package.json
[WARN] Error loading @capacitor/ios package.json: Error: Cannot find module '@capacitor/ios/package'

       Require stack:
       - C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli\lib\project\index.js
       - C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli\lib\index.js
       - C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli\index.js
       - C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli\bin\ionic
[WARN] Error loading @capacitor/android package.json: Error: Cannot find module '@capacitor/android/package'

       Require stack:
       - C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli\lib\project\index.js
       - C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli\lib\index.js
       - C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli\index.js
       - C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli\bin\ionic

Ionic:

   Ionic CLI                     : 6.20.8 (C:\Users\Administrator\AppData\Roaming\npm\node_modules\@ionic\cli)
   Ionic Framework               : not installed
   @angular-devkit/build-angular : 16.0.4
   @angular-devkit/schematics    : 16.0.4
   @angular/cli                  : 16.0.4
   @ionic/angular-toolkit        : 9.0.0

Capacitor:

   Capacitor CLI      : 5.0.4
   @capacitor/android : not installed
   @capacitor/core    : 5.0.4
   @capacitor/ios     : not installed

Utility:

   cordova-res : not installed globally
   native-run  : 1.7.2

System:

   NodeJS : v18.13.0 (C:\Program Files\nodejs\node.exe)
   npm    : 8.19.3
   OS     : Windows 10
```

## Additional Information

In my project:
- The homepage displays all devices, and the title of the homepage is named "Control Center".
![image](https://github.com/ionic-team/ionic-framework/assets/20255750/1a6f5397-6252-4de9-9620-a48becee9e03)

- Click on the device to enter the device details page. The text of the return button on the device details page is "Control Center" and the title is <device name>.
![image](https://github.com/ionic-team/ionic-framework/assets/20255750/1dcee3c0-6e48-46d9-93df-0c718f5498f9)

- Then click the settings icon in the upper right corner of the device details page to enter the device settings page. The back button text on the device's settings page is <device name>.
![image](https://github.com/ionic-team/ionic-framework/assets/20255750/b3e8f572-4da4-4ff4-bd6a-fa0da213aff3)
