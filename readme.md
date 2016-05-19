

## 大綱

整理自己，用過或是收集到的Library。

## 目錄

- [UI](#ui)
  - [未分類](#uncategory)
  - [Side ViewController](#side-viewcontroller)
- [SQLite](#sqlite)
- [Resources](#resources)
- [Log][#log]

## UI

### Uncategory

- [XLPagerTabStrip](https://github.com/xmartlabs/XLPagerTabStrip)  
  - 一個看起來很讚的custom tab元件。
- [SnapKit](https://github.com/SnapKit)	
  - 用Codes管理AutoLayout constraint。這個包的很漂亮，語法看來很容易使用。
- [OAStackView](https://github.com/oarrabi/OAStackView)
  - iOS 9有出一個UIStackView。但如果要在iOS 9之前的版本，使用類似的設計的話，就需要考慮這一個了。
- [AsyncDisplayKit](https://github.com/facebook/AsyncDisplayKit)
  - Facebook開發。後來獨立，並且Release的一個強大的UI元件。
  - 可以用Async的方式，預先準備好UI的內容，最後再呈現出來。這也是它強大的主要原因之一。用來讓UI反應更快速。可參考這個說明網頁。這東西要會使用，需要點時間，看它的說明文件…。"
- [Async](https://github.com/duemunk/Async)
  - Syntactic sugar in Swift for asynchronous dispatches in Grand Central Dispatch
  - 從它的說明範例看來，這個非常的好用。
- [DeviceKit](https://github.com/dennisweissmann/DeviceKit)
  - 用來查詢mobile device的狀態。像是機型、電池資訊等等。

### Side ViewController
- [SlideMenuControllerSwift](https://github.com/dekatotoro/SlideMenuControllerSwift)
  - 第一印象：
    - 看了幾個之後，這個最順眼。用Swift寫的元件。star數有破千了。
    - 依據專案的iOS SDK版本。選擇適合的branch使用。如swift2.1, swift1.1, swift1.2…。
    - 說明文件說，可直接支援**Storyboard**。這個元件的使用說明相對較完整。
    - [開發者Yuji Hato](https://github.com/dekatotoro)，是個日本人。大推。
  - 使用之後的心得
    - 雖然有支援Storyboard，但是一開始上手，還是需要花點時間，了解它怎麼被使用。
    - 它的動畫效果不是我要的。這才是我放棄的原因。這類的元件還不少，但是動畫效果，能不能和美工、主管們期待的一致，才會是關鍵。
    - 本來想跳下去修改它的程式碼。看了別人有幫他增加了segue的支援，但是原作者回文說，他不考慮加segue這東西進去。再用了另一個`SWRevealViewController`之後，就放棄幫忙這個選項了。因為心裡冒出了「頑固」這個單字。想一想之後還是放棄這個選項。

- [ENSwiftSideMenu](https://github.com/evnaz/ENSwiftSideMenu)
  - 也是用Swift寫的元件。star數有破千。
  - 目前v0.1.1，支援iOS 8以上。
- [SWRevealViewController](https://github.com/John-Lluch/SWRevealViewController)
  - 第一印象：
    - 用Obj-c寫的元件。**star數破3千多**。
    - 優點，可以support iOS SDK 7之後的專案。
    - 這個比較有名…。導至美工參考的App，是這個的實作。
  - 使用之後的心得
    - 它真的很方便。因為有提供UIStoryboard的支援。所以，不用寫什麼程式碼，就能完成它所呈現的特效效果。使用的方式，直接抓它的example看一看，很快就能上手了。但是進階一點的設定之類的，就需要花時間去Trace它的程式碼。
    - 客製化一些行為會比較麻煩一點。它的程式碼，覺得不容易閱講。是個陳舊，而且有很多人投入的專案。因為它是用Obj-C寫的，所以會帶有Obj-C的歷史包衭。

### Cover Flow
- [iCarousel](https://github.com/nicklockwood/iCarousel)
  - 第一印象：
    - 我看到的時候，star數己經是7k多了。
    - 提供多個模式可以使用。多種需求，都能用這個元件滿足。
    - [找到的教學文件，裡面是用Swift的語法，使用這個元件。](https://www.hackingwithswift.com/example-code/libraries/how-to-get-a-cover-flow-effect-on-ios)

### PageView Controller

局部的UI畫面，需要有page切換的效果。

### UICollectionViewLayout 相關
- [UICollctionViewLayout說明 1](https://onevcat.com/2012/08/advanced-collection-view/)
- [CHTCollectionViewWaterfallLayout](https://github.com/chiahsien/CHTCollectionViewWaterfallLayout)
  - 像瀑布一樣的Layout。看了一下，覺得很像Windows 8的一堆方塊牆。
- [MSCollectionViewCalendarLayout](https://github.com/erichoracek/MSCollectionViewCalendarLayout)
  - 像Calendar的Layout。目前用不到，但瞄了一下，覺得很強大。
    

### Progress
- [MBProgressHUD](https://github.com/jdg/MBProgressHUD)
- [MRProgress](https://github.com/mrackwitz/MRProgress)

### Popup
跳出Popup的小畫面。某些情形下，這個東西會很好用。
- [Popover](https://github.com/corin8823/Popover)
  - 提供了幾個樣式，可以參考。

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

## Resources
- [iOS Project study](https://www.raywenderlich.com/55384/ios-7-best-practices-part-1)
  - 裡面有介紹幾個，不錯的3rd party元件。
  - WebService。讀取JSON資料，轉換成App UI。
- Sub projects vs library
  1. http://www.galloway.me.uk/tutorials/ios-library-with-resources/
    - 一個Sample project。包含了Library的部份，和Application，引入Library的範例。它是用Static library。
- [Swift Style Guide](https://github.com/raywenderlich/swift-style-guide)
  - 快速上手Swift用的。
- [iOS Cookies](http://www.ioscookies.com)
  - iOS各種技術的大補帖？
  -『這個網站對iOS開發者很補, 用各種技術主題整理的相當好』"
- [Awesome Swift](https://github.com/matteocrippa/awesome-swift)
  - 聽說這個很厲害…。裡面會推薦很多Library，而且有分類。
- [3rd Party Library for iOS](https://github.com/iOSBeginner/3rd-Party-Library-for-iOS#ui-design)
  - 作者己經收集了，很多3rd party的Library。需要找東西，可以參考一下。
- [AppCoda](http://www.appcoda.com)  
  - 沒事可以來看一下。很多教學文件。可以當做看新聞，休閒娛樂用的。
- [code4app](http://www.code4app.net/index.html)
  - 找3rd party元件用的。

