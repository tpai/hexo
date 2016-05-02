---
layout: post
title: 'Google Cloud Platform + Bitnami'
date: 2014-11-14 16:22:00
categories: web
---

<iframe width="560" height="315" src="//www.youtube.com/embed/9AYB5Oq1kr0" frameborder="0" allowfullscreen></iframe>

最近在玩Cloud Service 發現Google跟Bitnami合作推出的這個solution還蠻方便的

提供了很多應用服務可以一鍵安裝 免除掉以往還要一個個裝 光搞設定就搞死了... Orz

[https://google.bitnami.com/](https://google.bitnami.com/)

Wordpress, Joomla, Drupal, Moodle, LAMP, nodejs, rubystack...等等

基本上你想得到的CMS、Environment這都有 所以何不give it a try呢 XD

當然在[document](http://wiki.bitnami.com)上 bitnami其實還有需要努力的空間

不過好在他們有相當不錯的[社群](https://community.bitnami.com/) 所以在QA上不會有太大問題

另外可以用[Google Developers Console](https://console.developers.google.com)去監控機器的請求量跟花費

這篇同時會用來記錄使用上所碰到的問題跟解法備忘

**remote ssh**

```
ssh -i bitnami.cer bitnami@<ip>
```

**sftp**

Use "bitnami" as username, use .cer file as password.

**remote access to phpmyadmin**

Create Tunnel

```
$ ssh -N -L 8888:127.0.0.1:80 -i bitnami.cer bitnami@<ip>
```

To: [http://127.0.0.1:8888/phpmyadmin](http://127.0.0.1:8888/phpmyadmin)

**convert .ppk to .pem**

```
$ brew install putty
$ puttygen privatekey.ppk -O private-openssh -o privatekey.pem
$ chmod go-rw privatekey.pem
$ ssh -i privatekey.pem user@my.server.com
```

Ref: [use-ppk-file-in-mac-terminal-to-connect-to-remote-connection-over-ssh](http://stackoverflow.com/questions/3475069/use-ppk-file-in-mac-terminal-to-connect-to-remote-connection-over-ssh)

