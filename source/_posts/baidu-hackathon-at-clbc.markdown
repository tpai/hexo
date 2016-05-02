---
layout: post
title: 'Baidu Hackathon 2013'
date: 2013-07-29 10:59
categories: hackathon
---
![百度開發雲編程馬拉松](http://i.imgur.com/Jed1G37.jpg)

貴為當兵前最後一次黑客松 真的是既感慨又感動啊...

<!--more-->

這次的作品iBulb的誕生結合了本次黑客松的主題「綠色生活」

以及[幻騰智能](http://huantengsmart.com/intro)所提供的LED燈泡

後端透過nodejs對官方所提供的燈泡api做request (亮度及色溫調整

```
$.ajax({
    type: "POST",
    url: "/set",
    dataType: "json",
    data: {
        turned_on: true, //開關
        brightness: data.brt, //亮度 0-1
        hue: data.hue //色溫 0-1
    },
    success: function (result) {
        console.log(result)
    }
})
```

前端則是參考 @stevechiou 所提供的[樣板網站](http://iweb-studio.com/wrapbootstrap/maxim/)來進行重製

![首頁](http://i.imgur.com/4N9OwHG.png)

![關於團隊](http://i.imgur.com/mEVLQyn.png)

![情境模擬](http://i.imgur.com/JnjeLKP.png)

同時呢 除了iBulb這個作品之外 我們還另外設計了一個小遊戲 (杰哥:比遊戲還刺激

至於這遊戲呢 本來打算只是讓它扮演demo過程中的一段小插曲 但是後來發現效果拔群 XD

遊戲的靈感來自於省電

話說電力早已成為人們生活中不可或缺的部分

而人們也覺得電力的使用與獲得是天經地義的

因此我們想試著讓大家去體驗電力的取得是很辛苦的

大家對腳踏車發電還有印象吧? (靈感來自[漂流教室](http://www.8comic.com/210.html)

不過腳踏車什麼的對阿宅來說是八輩子碰不著的東西啊啊啊 XDDD

最近不是很流行鍵盤什麼的嗎? 那我們就來個「鍵盤發電機」吧 :D

![鍵盤發電機](http://i.imgur.com/AjCqxeZ.png)

大家一起拼命的連擊左右鍵來讓電力慢慢地上升吧!!! 直到燈泡射出它完全的100%的亮度!!! >///<

這樣一來既喚醒大家的節能意識 也同時可以讓許多玩家共同體驗電力的獲得是多麼的辛苦 (這遊戲存在本身是浪費電啊啊啊 XDD

最後呢 也很幸運的獲得評審的青睞 得到人氣創意獎

很感謝好隊友的幫忙與合作才有這次的成果 特別感謝 @stevechiou @vansdog

![人氣創意獎](http://i.imgur.com/1J9Zm8U.jpg)
