
## 目錄
  - [SQLite](#sqlite)
  - [Log](#log)
  - [Zip](#zip)

## SQLite
  - [SQLite.swift][sqlite.swift]
    - 看起來不錯。在特色裡面，有一項[Well-documented](https://github.com/stephencelis/SQLite.swift/blob/master/Documentation/Index.md#sqliteswift-documentation)
  - [SQLiteMigrationManager](https://github.com/garriguv/SQLiteMigrationManager.swift)
    - 可以搭配[SQLite.swift][sqlite.swift]使用。版本有點新，覺得還有進化的可能。
    - 以目前看到的程式，如果只有一個.sqlite的話，應該是夠用的。怎麼說呢…？像MS的Entity Framework，在2014之前，它的migration可以支援多個db的行為。那個migration table需要額外記一些東西。目前的SQLiteMigrationManager(v0.0.5)還沒有這個能力。一般而言是不會有這個需求的。只是看了一下程式碼，得到的心得。

[sqlite.swift]: https://github.com/stephencelis/SQLite.swift

## Log
- [CocoaLumberjack](https://github.com/CocoaLumberjack/CocoaLumberjack)
  - 有Obj-C。
  - 在ObjC用過，還蠻不錯的。也可以設定多種Log的方式。和自定Log Level。
  - Swift下，似乎不太一樣就是了。
- [CleanroomLogger](https://github.com/emaloney/CleanroomLogger)
  - 純Swift。瞄了一下，它做的也不錯。
  - 該有的東西都有…。
  - 還蠻新的，我看到的時候，star數還沒破千。可是CocoaLumberjack己經7千多了。這個值得期待，但現階段可以觀望一下。
- [PlCrashReporter](https://www.plcrashreporter.org)

### Crash report related
- [Overview of iOS Crash Reporting Tools: Part 1](https://www.raywenderlich.com/33669/overview-of-ios-crash-reporting-tools-part-1)
  - 雖然只是Part I。但是提供了不少，要付費，也有些是免費的Crash Report的服務。
  - 最後建議，在iOS上使用Crashlytics。找了其它的文章，它被Twitter收購。而且，[似乎保障它是免費的](http://www.crashlytics.com/blog/crashlytics-enterprise-is-now-free/)。
  - [Crashlytics, docs](https://docs.fabric.io/ios/crashlytics/crashes-and-issues.html)
- [QuincyKit](https://github.com/bitstadium/QuincyKit)
  - 這個，需要自己架Server。[從Stackoverflow上撿來的](http://stackoverflow.com/a/11313132/419348)。
- [Google Anylytics for iOS](https://developers.google.com/analytics/devguides/collection/ios/v3/?ver=swift#get-config)  
  - 呃…Google耶

## Zip
- [ZipArchive](https://github.com/mattconnolly/ZipArchive)
  - ZipArchive的名稱還蠻多人用的呀。這個是專案有用到的。都會用到*minizip*這個。
- [ZipArchive](https://github.com/ZipArchive/ZipArchive)  
  - SSZipArchive
  - 也是會用到*minizip*。看來，也是再包一層。

## Cache
- [TMCache](https://github.com/tumblr/TMCache/)
  - [它將不會繼續維護了。有點可惜。](https://cocoa.tumblr.com/post/118790665043/tmcache-is-no-longer-being-actively-maintained)