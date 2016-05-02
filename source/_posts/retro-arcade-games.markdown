---
layout: post
title: 'Retro Arcade Games'
date: 2014-11-26 18:01
categories: acgm
---

話說我國小時正好是大型街機的全盛時期呢~

真的很懷念那段打街機 圍觀神手電人的時光 (遠目)

<iframe src="//www.slideshare.net/slideshow/embed_code/41863897" width="800" height="600" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe>

為了找回來玩 稍微費了點功夫做了田野調查(?)

想玩的朋友歡迎一起來當老人懷舊一下吧 XDDD

**Windows**

* [mame](http://mamedev.org/release.html)

**Mac OSX**

* [mameosx](http://mameosx.sourceforge.net/) (UI)
* [sdlmame](http://sdlmame.lngn.net/) (Console)

UI版基本上只要設定好ROMs資料夾的位置，就沒什麼問題了。

比較會有問題的是console，直接執行的話會出現下列錯誤訊息。

    dyld: Library not loaded: @rpath/SDL.framework/Versions/A/SDL
    Referenced from: ~/mame0155-32bit/./mame
    Reason: image not found

意思就是缺少SDL Library，但問題就是要怎麼解決呢？

1. [SDL 1.2](http://www.libsdl.org/download-1.2.php)
2. Download the latest SDL-1.2.x.dmg
3. Open /Library/Frameworks/.
4. Drag SDL.Framework from SDL disk image into that folder.
5. ./mame

Ref: [Trying to run SDLMame on Mac OSX](http://www.mameworld.info/ubbthreads/showflat.php?Cat=&Number=246819&page=0&view=expanded&sb=7&o=&vc=1)
