
## 目錄
  - [SQLite](#sqlite)
  - [Log](#log)

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