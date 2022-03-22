# RPG-DICE-GAME
自製-RPG骰子戰鬥系統(RPG-DICE-GAME)

## 實作目的
在軟體專案管理的課程中，需要規劃一個專案，<br>
而當時在練習C# WPF，想藉由課程專案來完成小時候就嚮往製作遊戲的一個夢想。<br>

## 設計理念與技術
構想來自於網路上某資工製作的期末作品，<br>
屬於大富翁的遊戲風格，我將它與現代回合制RPG結合並加以改良完成，<br>
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

## 相關程式畫面
### 開始畫面<br>
<img src="https://github.com/lfre84216/RPG-DICE-GAME/blob/main/1.png">
<br>

### 關卡選擇畫面<br>
<img src="https://github.com/lfre84216/RPG-DICE-GAME/blob/main/2.png">
<br>

### 骰子人物行走畫面<br>
<img src="https://github.com/lfre84216/RPG-DICE-GAME/blob/main/3.png">
<br>

### 武器店畫面<br>
<img src="https://github.com/lfre84216/RPG-DICE-GAME/blob/main/4.png">
<br>

### 藥水店畫面<br>
<img src="https://github.com/lfre84216/RPG-DICE-GAME/blob/main/5.png">
<br>

### 戰鬥畫面<br>
<img src="https://github.com/lfre84216/RPG-DICE-GAME/blob/main/6.png">
<br>

### 遊戲影片DEMO展示
[![IMAGE ALT TEXT HERE](https://github.com/lfre84216/RPG-DICE-GAME/blob/main/%E9%81%8A%E6%88%B2%E6%A8%99%E9%A1%8C%E8%83%8C%E6%99%AF.JPG)](https://www.youtube.com/watch?v=EHohVcn1hmE)

## 製作過程與困難點
在實作該專案的過程中，其實遇過很多問題，<br>
像是控制項的動畫效果，以及戰鬥系統的設定<br>
主要都是使用多執行緒的概念來進行實作，<br>
並且透過委派(Delegate)的方式，委託UI執行緒來對控制項非同步操作，<br>
即可達成上述等功能的實現。<br><br>
另外在進行擲骰子後進行的走路動畫也思考了很久，<br>
寫出了一個類走路動畫的演算法，<br>
在走到第n格時，對n和n-1格進行動畫的顯示與消失，也是透過多執行緒實作，<br>
算是蠻有成就感的一件事。<br>
