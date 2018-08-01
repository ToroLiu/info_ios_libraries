
## 目錄
  - [SQLite](#sqlite)
  - [Log](#log)
  - [Zip](#zip)
  - [Cache](#cache)

## SQLite
  - [SQLite.swift][sqlite.swift]
    - 看起來不錯。在特色裡面，有一項[Well-documented](https://github.com/stephencelis/SQLite.swift/blob/master/Documentation/Index.md#sqliteswift-documentation)
    - 有載了`SugarRecord`，看了一下之後，覺得CoreData如果不常用的話，上手所需要的時間。還在猶豫要不要投資這項技術。
  - [SQLiteMigrationManager](https://github.com/garriguv/SQLiteMigrationManager.swift)
    - 可以搭配[SQLite.swift][sqlite.swift]使用。版本有點新，覺得還有進化的可能。
    - 以目前看到的程式，如果只有一個.sqlite的話，應該是夠用的。怎麼說呢…？像MS的Entity Framework，在2014之前，它的migration可以支援多個db的行為。那個migration table需要額外記一些東西。目前的SQLiteMigrationManager(v0.0.5)還沒有這個能力。一般而言是不會有這個需求的。看了一下Github的程式碼，得到的心得。
  - [SugarRecord](https://github.com/carambalabs/SugarRecord)
    - 以前有看到過。這次心血來潮，又找了一下CoreData ORM，找到這個。star數有破千了。應該是值得期待的一個3rd party框架吧。
    - 支援Swift3的語法。
    - Storage的部份，除了SQLite之外，還整合了iCloud，和Realm。

[sqlite.swift]: https://github.com/stephencelis/SQLite.swift

## Log
- [XCGLogger](https://github.com/DaveWoodCom/XCGLogger)
  - 適合Swift的Log系統。CocoaLumberjack覺得有點陳舊了，之前想整合Crashlytics的Log系統，總是有些問題。希望XCG這個會比較好一點。
  - 目前只是觀望，從文件上覺得這個還蠻值得期待，但還沒有使用過。
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
  - 從上述這篇，TMCache有推薦使用PINCache。如果有需要的話…。
- [PINCache](https://github.com/pinterest/PINCache)  
  - 從TMCache fork出來的。TMCache有thread starvation的問題。從PINCache這邊的說法，如果重度使用TMCache的話，會有dead lock的問題。
- [SDWebImage](https://github.com/rs/SDWebImage)
   - Star數相當的高，有蠻多人關注和使用。
   - 瞄了一下。這拿來處理Image cache，會非常好用。大多數的Cache，應該都是和Image cache有關係吧…。
- [Cache](https://github.com/hyperoslo/Cache)
   - 後來捨棄了`TMCache`，改用了這一套。它和Swift的`Codable`搭配起來，很多事情變的很簡單。
- [Imaginary](https://github.com/hyperoslo/Imaginary)
   - 這個是用來處理Image cache。它提供了一些方便的寫法，擴充了UIImageView的功能。使得從URL取影像變的簡潔多了。而背後的快取和加速之類的，它會幫你處理掉。
   - 和上面那個Cache是同個作者寫的，底層也是用`Cache`當成影像快取。

## String
- [BonMot](https://github.com/Raizlabs/BonMot)
   - 唸成Bon Mo，是法文，指的是Good Word。
   - AttributedString的加強版，讓套用Style的語法變的簡潔。然後套用圖檔似乎也比較容易一些。比較特別的是，它可以用來處理一些自定義的XML tag。針對那些tag套用自己定義的style。
   - 用了之後，可能最近升級到Xcode 9.2的關係，照著文件上的語法敲了幾次，編譯過不了。最後放棄。
- 關於NSAttributedstring的處理
  它有個簡易的方式可以將html的字串，轉成相對應的attributedString。這方法很容易找到，而且也沒幾行，很適合包成一個小小的Utility function。然後呢，它也會處理html裡的css style。所以可以在程式裡面，將css寫在html string之前，這樣就能套用客製化的App style了。

