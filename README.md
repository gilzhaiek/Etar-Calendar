Etar (from Arabic:  `إِيتَار`) is an open source material designed calendar made for everyone!

<a href="https://itunes.apple.com/us/app/etar/id1217625781?mt=8"><img src="https://upload.wikimedia.org/wikipedia/commons/5/5d/Available_on_the_App_Store_%28black%29.png" width="150"></a>

![Etar Calendar](./assets/_pre_prod/publish/v1.0/animation.gif)

##Why?
Well, I wanted a simple, material designed and state of the art open source calendar that anyone can make it better.

##Special thanks

The application is an enhanced version of AOSP Calendar. Without the help of
[Free Software for Android](https://github.com/Free-Software-for-Android/Standalone-Calendar) team, 
this app would be just a dream. So thanks to them!

##Features
- Month view.
- Week, day & agenda view.
- Uses Android calendar sync. Works with Google Calendar, Exchange, etc.
- Material designed.
- Agenda widget.

### Build instructions
```
git submodule init
git submodule update

gradle build
```

### How this was done
- see ``build.gradle`` and the modifications to ``AndroidManifest.xml``
- ``fix_strings_and_import.py`` was created to fix a build problem and rename imports of R.java
- get time zone data from http://www.iana.org/time-zones write ``backward`` and ``zone.tab`` to assets and to assets of https://github.com/dschuermann/standalone-calendar-timezonepicker
- comment out code in https://github.com/dschuermann/standalone-calendar-frameworks-ex
