
## 目錄
- [未分類](#uncategory)
- [Side ViewController](#side-viewcontroller)
- [Cover Flow](#cover-flow)
- [PageView Controller](#pageview-controller)
- [UICollectionViewLayout相關](#uicollectionviewlayout-相關)
- [Progress](#progress)
- [Slide Bar](#slide-bar)
- [Popup](#popup)

- [UITableView](#uitableview)
- [Pull Refresh](#pull-refresh)

- [Switch](#switch)
- [Misc](#misc)

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
  - 因為又要用到，所以又連到github上看一下怎麼使用。有好幾個知名的iOS開發部落格，寫文章介紹這個元件，怎麼使用。    

### Cover Flow
- [iCarousel](https://github.com/nicklockwood/iCarousel)
  - 第一印象：
    - 我看到的時候，star數己經是7k多了。
    - 提供多個模式可以使用。多種需求，都能用這個元件滿足。
    - [找到的教學文件，裡面是用Swift的語法，使用這個元件。](https://www.hackingwithswift.com/example-code/libraries/how-to-get-a-cover-flow-effect-on-ios)

### PageView Controller

局部的UI畫面，需要有page切換的效果。
- [EAIntroView](https://github.com/ealeksandrov/EAIntroView)
   - 別人用來客製，App一開始的Introduction pages用的。看起來蠻有趣的。

- [PageControl](https://developer.apple.com/library/ios/samplecode/PageControl/Introduction/Intro.html#//apple_ref/doc/uid/DTS40007795)
  - Apple的sample code，示範怎麼使用UIScrollView, 和UIPageControl。做出page的效果。

### UICollectionViewLayout 相關
- [UICollctionViewLayout說明 1](https://onevcat.com/2012/08/advanced-collection-view/)
- [CHTCollectionViewWaterfallLayout](https://github.com/chiahsien/CHTCollectionViewWaterfallLayout)
  - 像瀑布一樣的Layout。看了一下，覺得很像Windows 8的一堆方塊牆。
- [MSCollectionViewCalendarLayout](https://github.com/erichoracek/MSCollectionViewCalendarLayout)
  - 像Calendar的Layout。目前用不到，但瞄了一下，覺得很強大。
- [CSStickyHeaderFlowLayout](https://github.com/jamztang/CSStickyHeaderFlowLayout)  
  - 看起來蠻厲害的。它的star數相當的高。
  - 也是實作出像UITableView的樣子，但做了更多的客製化效果。
- [PDKTStickySectionHeadersCollectionViewLayout](https://github.com/Produkt/PDKTStickySectionHeadersCollectionViewLayout)  
  - 值得參考的一個範例。它實作出和UITableView和相似的行為，然後由protocol決定，section是否要黏在上面。
- 教學文件
  - https://www.raywenderlich.com/107439/uicollectionview-custom-layout-tutorial-pinterest
    - 看完上面這篇，它提供的其它連結
      - [Creating Custom Layouts](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/CollectionViewPGforIOS/CreatingCustomLayouts/CreatingCustomLayouts.html)
  - [UICollectionView class reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UICollectionView_class/)
    - 這個頁面，會說明什麼是`Decoration view`，和`Supplementary view`


### Progress
- [MBProgressHUD](https://github.com/jdg/MBProgressHUD)
- [MRProgress](https://github.com/mrackwitz/MRProgress)

### Slide Bar
- [How To Make a Custom Control Tutorial: A Reusable Slide](https://www.raywenderlich.com/76433/how-to-make-a-custom-control-swift)
   - raywenderlich裡的教學文章。教你怎麼繼承`UIControl`，打造自己的UI元件。
- [How to Implement Custom UISlider in Swift](http://www.alexanderbatalov.com/journal/2015/2/20/how-to-implement-custom-uislider-in-swift)   
   - 這一篇是使用UISlider，並且套用客製化後的圖…。

### Popup
跳出Popup的小畫面。某些情形下，這個東西會很好用。
- [Popover](https://github.com/corin8823/Popover)
  - 提供了幾個樣式，可以參考。
  - 還蠻好用的。在計算start point需要小心一些。

### UITableView
- [MGSwipeTableCell](https://github.com/MortimerGoro/MGSwipeTableCell)
  - 如果有需要的話，要參考這邊的實作…。可以Swipe的Cell。
- [Self-sizing Table View Cells](https://www.raywenderlich.com/129059/self-sizing-table-view-cells)  
  - 動態調整高度的Cell。這邊的AutoLayout很強大呀。

### Pull Refresh
下拉更新的UI元件。

- [DGElasticPullToRefresh](https://github.com/gontovnik/DGElasticPullToRefresh)
  - 找支援Swift3，可以下拉更新的UI元件時，找到這一個。因為最近Apple釋出Swift3，本來這類的元件很多，但是有支援Swift3的不多就是了。

### Charts
- [Charts](https://github.com/danielgindi/Charts)  
  - 功能應該很強大。star數看到的時候己經九千多了…。
  - 因為很強大，所以難以理解和學習吧…。
- [SwiftChart](https://github.com/gpbl/SwiftChart)
  - 開發沒多久的一個Library。看起來簡單多了…。比較適合拿來修改？
- [JBChartView](https://github.com/Jawbone/JBChartView)
  - Obj-C所寫成的。因為Fabric的App有引入這個License，所以就拿來看一下。

### Switch
因為iOS的UISwitch，它的size是固定的。可是客製後的UI，size通常不太一樣，於是就有客製化的Switch的需求。
- [SevenSwitch](https://github.com/bvogelzang/SevenSwitch)
  - Google找到的，然後是用Swift語法寫成。看了一下，算是符合需求了。
  - 原作者沒有繼續維護。有些可惜。目前沒有支援Swift3。有人fork後，另外整理成支援Swift3了。

### MISC
- [CRToast](https://github.com/cruffenach/CRToast)
  - 用來客製化Notification UI的效果，感覺會很好用。
  - 在iOS 10，Notification的框架有改變。有系統的Framework可以呈現Notification UI。而且，花樣也變多了，支援更多的格式，用來呈現Notification。
- [EasyTipView](https://github.com/teodorpatras/EasyTipView)  
  - 用來呈現，App的使用教學。可以顯示一個小小的Tip。看了一下，感覺還蠻漂亮的。
  - EasyTipView is a fully customizable tooltip view written in Swift that can be used as a call to action or informative tip.
  - MIT License
-  [FLEX](https://github.com/Flipboard/FLEX)
  - 一個很神奇的Debug tool。它是In-app的。在UIWindow上會有一個按鈕，可以把它叫出來。似乎能任意的調整UI的properties，看system log，還有network request&response…。還能看SQLite資料庫!??感覺很神奇。
- [JLRoutes](https://github.com/joeldev/JLRoutes)
  - 又是個神奇的東西。怎麼會有人，想到把`front view controller`的概念，搬到iOS dev上呢。這是用來實現，現在常見的網頁MVC架構的神奇工具呀。iOS可以吃openURL的東西，通常是別的App呼叫自己的App時，會使用URL傳東西過來…。有這個Library，可以讓這類型的開發，整個變的容易，好管理。寫過asp.net MVC/WebAPI，或是Django之類的，應該會很有感覺吧。
- [FlatUIKit](https://github.com/Grouper/FlatUIKit)  
  - 為了繪製自己的SliderBar，後來找到這一個。它裡面有`UIImage+FlatUI`的extension，可以幫忙繪製出`UISlider`所需要的圖。還有其它`UIKit`的extension，看起來也不錯用。是個值得花時間，閱讀一下的3rd party程式碼。
- [DeviceKit](https://github.com/dennisweissmann/DeviceKit)  
  - 為了解決一個需求，想知道用戶的iPhone的型號，像是iPhone 5s, iPhone 6 plus之類的資訊，於是找到這一個東西。
  - 它支援Swift3的語法唷。
- [SwiftRichString](https://github.com/malcommac/SwiftRichString)  
  - Attributed Strings的Library。可以讓字串的各種Style的套用，變的很優雅。
  - 看完了一開始的簡介，Easy Styling，我就迷上這個Library了。用它來處理字串中套用各種的Style變的很簡單。
