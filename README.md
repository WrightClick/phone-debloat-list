## phone-debloat-list
Phone debloat list is a text file that contains adb (android device bridge) commands
to disable system / user apps deemed as bloatware, often installed on phones by carriers
such as AT&T, verizon, etc. Often, there are unneeded bloatware apps from Google too,
such as Google Books, News, etc.

This set of commands will disable these packages and system apps, removing all of the junk
not needed.

##*Warnings*
Just so you know, this list disables Google Play Services and anything that runs off of it.

This means that the Google Play Store, Youtube, Gmail, etc. will not function, you will not be able to download apps from the play store, you will not be able to login into any app that uses Google's OAuth platform for authentication, etc. **ANYTHING** remotely tied into Google or Samsung will break.

Workarounds for this include:
1. Browsing youtube through a web browser
2. Enabling unsecure app access through your Google account settings (then using a third party email app, I recommend *FairEmail* on FDroid / Aurora Droid.
3. Learning to enjoy a reduced dependency on social media / apps.


##*Prerequisites*
1. Ensure that you have a third party web browser (Bromite is recommended)
2. Ensure that you have a third party phone app (This list excludes the phone app, but just to make sure)
3. Ensure that you have a third party text/sms app
4. Ensure that you have a third party camera app
5. Ensure that you understand how to install / sideload apps (This list disables Google Play Services) or use a third party repo for apps (FDroid / Aurora Droid) for installing free and open source apps

######*How to use*
To use this list, you must have adb debugging enabled for your device. To do this, see below.
1. Enter device shell by executing 'adb shell'
2. Pick the list you want, and copy and paste them into the shell. The shell will begin executing them, but will stop on the last command. Just press enter to run the last one. If the package was disabled, you will see "success" after each command runs, otherwise you will see an error (usually just that you dont have the package installed to begin with.
3. Once done running the commands desiered from the list, close the shell window.
4. Disconnect the device, reboot.
5. Profit.
