FakeWifi
==================
**This app is no longer maintained, as I have no use for it and no way to test it. Pull requests are still welcomed, altough nobody really cared to make them yet.**

Make android apps believe Wifi is connected.

Handy in situations where there is a (non wifi) connection, but some app won't do its thing unless it's on wifi
( android running in virtual machine / emulator, 3g but no wifi around, usb 3g modem connection, usb reverse tethering, device with ethernet, ...)

With this you can for instance access wifi-only features while on 3g/Ethernet, etc.

Tested on Android 4 (KitKat) and 6 (Marshmallow).

No app is faked by default. Open FakeWifiConnection app to enable/disable hack (master switch) and select which apps to fake.

Install
-------
Prerequisites: *Xposed Framework.*

- Install [Fake Wifi from Google Play](https://play.google.com/store/apps/details?id=eu.chylek.adam.fakewifi) or build and install from source.  
- Open Xposed Installer->Modules, tick Fake Wifi  
- Reboot
- Open Fake Wifi app to change settings.

Debugging
---------

Debug messages are disabled by default and shouldn't be needed. Enable them in the GUI if you want.

`logcat | grep FakeWifi`

Also check Xposed logs:

`logcat | grep Xposed`

Credits
-------

- rovo89 for awesome Xposed Framework
- lemonsqueeze for [the original version of this app](https://github.com/lemonsqueeze/FakeWifiConnection/)
- apsun for [Remote preferences](https://github.com/apsun/RemotePreferences)

Like the app?
-------
Spread the word on the interwebs, tell your friends or donate to bitcoin wallet: 16AhXUfdozHEmnmWuDyHXVr4peXdj21irg

Released under [GNU GPL License](https://raw.github.com/chylek/FakeWifi/master/LICENSE).
