---
layout: post
title: 'NPAPI is coming to the end.'
date: 2014-11-05 16:15:00
categories: web
---

Netscape Plugin API = NPAPI

為什麼會提到這個？

因為Unity Blog上的一篇文章

[The Future of web publishing in Unity](http://blogs.unity3d.com/2014/10/28/the-future-of-web-publishing-in-unity-an-update/)

述說著Chrome即將要把NPAPI送入歷史 而Unity要何去何從

這對於我這個Chrome的重度用戶加Unity開發者來說當然是值得注意的消息

根據chromium blog在2013年中所發佈的[文章](http://blog.chromium.org/2013/09/saying-goodbye-to-our-old-friend-npapi.html)

Chrome 將從2014年初開始停止支援NPAPI，除了下列較常用的白名單之外：

* Silver Light
* Unity
* Google Earth
* Java
* Google Talk
* Facebook Video

這個流程預計將於2014年末達到完全終止對NPAPI的支援

根據這篇[NPAPI Deprecation](https://sites.google.com/a/chromium.org/dev/developers/npapi-deprecation)所述

接下來的幾次更新

前期會透過徵求user permission

中期會用block的方式

藉此引導開發者跟使用者走向新技術

替代方案的部分當然也是有的

第一個就是Google自家的Native Client (NaCL)

另一個就是呼聲很高的WebGL

至於Unity呢 根據文內的說法是打算朝向WebGL前進

當然也有在WebGL上做[效能評測報告](http://blogs.unity3d.com/2014/10/07/benchmarking-unity-performance-in-webgl/)

內容涵蓋3D物理、2D物理、粒子特效、動畫、物件生成、腳本及Draw Call等等測試

有興趣測試的可以打開[WebGL Benchmark](http://beta.unity3d.com/jonas/WebGLBenchmark/)玩玩

等到WebGL大盛之後 應該就不用裝上述那堆plugin了吧 :P

話說在那張跑分圖表中比較令我納悶的是Chrome的分數明顯比Firefox低了許多

後來查了一下 [arewefastyet.com](http://arewefastyet.com/#machine=11&view=breakdown&suite=asmjs-apps) 才發現Firefox **with asm.js**才會比較快

出於擔心也稍微找了一下有沒有Chrome跟進的消息

[來自Mozilla Bog的文章](https://blog.mozilla.org/futurereleases/2013/11/26/chrome-and-opera-optimize-for-mozilla-pioneered-asm-js/)說明Chrome跟Opera也有逐步在跟進asm.js與WebGL技術

這對開發者來說 應該算是好消息吧 :D
