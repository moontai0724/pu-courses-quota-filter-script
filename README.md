# 靜宜大學 課程清單 人數顯示與過濾

## 前言

剛上大學，發現要一個一個查課程剩餘人數還真是有點麻煩，所以寫了這小腳本。

建議縮小範圍之後再獲取人數，因為如果列表太多課程的話，處理會需要一段時間。

為了不要讓大家過於星爆，一直點擊送出大量請求，因此點一次之後會有 5 秒的冷卻時間，要等待 5 秒後才能再點。

雖然人數放在上課班級旁邊好像有點奇怪，但是多一個欄位的話有點麻煩，其他的欄位有點滿，那個位置剛好比較空也不小，所以就放在那裏了。

## 如何安裝？

前置需求：**建議**安裝 Tampermonkey ([Chrome](https://chrome.google.com/webstore/detail/dhdgffkkebhmkfjojejmpbldmpobfkfo)) ([Firefox](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey)) ([Safari](https://safari.tampermonkey.net/tampermonkey.safariextz)) ([Edge](https://www.microsoft.com/store/apps/9NBLGGH5162S))
下載頁面：[]()

安裝好擴充功能後，點進下載頁面，然後點選　`安裝腳本`，然後按確定即可。  
相關設定請繼續往下看。  

## 腳本說明

此腳本在安裝後，在課程清單網頁的最上面列表中會有一個「獲取目前修課人數」的選項：
![https://imgur.com/Wzq0N1E](https://imgur.com/Wzq0N1E.png "獲取目前修課人數的新增按鈕")

剛剛那個按鈕，在點下去之前是不會顯示人數的，這是為了避免在尖峰時段造成伺服器壓力。
![https://imgur.com/VLOa28v](https://imgur.com/VLOa28v.png "在點按鈕之前的狀況")

按下去之後就會顯示了，如果沒有課程代碼就不會顯示，附帶一提有些課程顯示 0 的那本來就是它顯示那樣的，應該是沒有上限的意思。
![https://imgur.com/p0ThNMn](https://imgur.com/p0ThNMn.png "在點按鈕之後的狀況")

## 相關連結

靜宜大學課程清單（選課手冊暨課程綱要查詢）：[http://alcat.pu.edu.tw/2011courseAbstract/main.php](http://alcat.pu.edu.tw/2011courseAbstract/main.php)
靜宜大學修課人數查詢：[http://alcat.pu.edu.tw/choice/q_person.html](http://alcat.pu.edu.tw/choice/q_person.html)
