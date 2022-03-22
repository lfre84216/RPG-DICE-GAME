# RPG-DICE-GAME
自製-骰子戰鬥系統(RPG-DICE-GAME)

## 實作目的
在軟體專案管理的課程中，需要規劃一個專案，<br>
而當時在練習C#，想藉由課程專案來完成小時候就嚮往製作遊戲的一個夢想。<br>
構想，<br>
而另外一方面則是可以加強自己對於實作專案的熟悉度。

## 設計理念與技術
構想來自於網路上某資工製作的期末作品，<br>
屬於大富翁的遊戲風格，我將它與現代回合制RPG結核病加以改良完成，<br>
主要利用骰子去決定角色移動的格數，每個定點上都有不同的設置機關，<br>
像是怪物、藥水店、武器店、超級怪物、特殊任務等，<br>
因此只要擲出不同的骰子點數，就能讓玩家有不同的體驗，使遊玩更具有互動性。<br>
- C# WPF應用程式
- Multi-Thread
- XAML
- WMPLib-WindowsMediaPlayer

## 主要實作功能
實作功能包含大富翁的整個移動系統，加上藥水武器的功能與介面，<br>
能夠進行全部的RPG運行流程。
- 完整遊戲流程(進行骰子移動->進入特定機關->打贏超級怪物->進入下一個part環節)
- 大富翁人物行走動畫
- 多執行緒戰鬥系統
- 委派UI執行緒執行控制項個別動畫
- 鍵盤滑鼠事件互動
- WPF多介面資料互動
- 實際RPG與音效圖片流程的配合
- 建構子初始化地圖物件

## 程式影片
<iframe width="560" height="315" src="https://www.youtube.com/embed/EHohVcn1hmE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## 相關程式畫面
### 登入註冊<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/7.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/8.png">
<br>

### 使用者介面<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/1.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/2.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/3.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/4.png">
<br>

### 管理者介面<br>
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/5.png">
<img src="https://github.com/lfre84216/BookBorrowSystem/blob/main/6.png">
<br>

## 製作過程與困難點
在實作該專案的過程中，有嘗試想要實際讓資料庫可以被外部來連接，<br>
達成實際直接遠端資料庫的功能，<br>
所以在網路這方面有另外研究了關於虛擬伺服器的功能，<br>
讓實作出來的程式也能透過外部裝置來進行連線。
