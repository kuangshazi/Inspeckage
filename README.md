# <img src="http://i.imgur.com/dupvus6.png" width="100" /> Inspeckage - Android Package Inspector

Inspeckage is a tool developed to offer dynamic analysis of Android applications. By applying hooks to functions of the Android API, Inspeckage will help you understand what an Android application is doing at runtime. 

Features
---------------

With Inspeckage, we can get a good amount of information about the application's behavior:

#### Information gathering 

* Requested Permissions;
* App Permissions;
* Shared Libraries;
* Exported and Non-exported Activities, Content Providers,Broadcast Receivers and Services;
* Check if the app is debuggable or not;
* Version, UID and GIDs;
* etc.

#### Hooks (so far)

With the hooks, we can see what the application is doing in real time:

* Shared Preferences (log and file);
* Serialization;
* Crypto;
* Hashes;
* SQLite;
* HTTP (an HTTP proxy tool is still the best alternative);
* File System;
* Miscellaneous (Clipboard, URL.Parse());
* WebView;
* IPC;
* + Hooks (add new hooks dynamically)

#### Actions

With Xposed it's possible to perform actions such as start a unexported activity and much else:

* Start any activity (exported and unexported);
* Call any provider (exported and unexported);
* Disable FLAG_SECURE;
* SSL uncheck;
* Start, stop and restart the application.

#### Extras

* APK Download;
* View the app's directory tree;
* Download the app's files;
* Download the output generated by hooks in text file format;
* Take a screen capture;

#### Configuration

Even though our tool has some hooks to the HTTP libraries, using an external proxy tool is still the best option to analyze the app's traffic. With Inspeckage, you can:

* Add a proxy to the target app;
* Enable and disable proxy;
* Add entries in the arp table.

#### Logcat

Logcat.html page. A experimental page with websocket to show some information from the logcat.

Installation
---------------
Requirements:
Xposed Framework

##### Xposed Installer

1. Go to Xposed Installer, select "Download"
2. Refresh and search for "Inspeckage"
3. Download the latest version and install
4. Enable it in Xposed
5. Reboot and enjoy!

##### Xposed Repository

Get it from Xposed repo: http://repo.xposed.info/module/mobi.acpm.inspeckage

        adb install mobi.acpm.inspeckage.apk
1. Enable it in Xposed
2. Reboot and enjoy!

##### From Source

Feel free to download the source!

### How to uninstall

        adb uninstall mobi.acpm.inspeckage.apk
And reboot!

## Genymotion

[![Genymotion](http://i.imgur.com/2bjhFn2.png)](https://vimeo.com/156745941)

### Screenshots

<img src="http://i.imgur.com/W7496ru.png" width="800" />

<img src="http://i.imgur.com/kdlajWg.png" width="900" />

<img src="http://i.imgur.com/CC4Qgem.png" width="900" />

<img src="http://i.imgur.com/FH7GifA.png" width="900" />

<img src="http://i.imgur.com/Lc6lHNB.png" width="900" />


License
-------

Copyright 2016 ac-pm

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
