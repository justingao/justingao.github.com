---

title: Android SDK Manager 无法更新
layout: post
categories: [Android]
tags: [ADT, Android]

---

使用 Android SDK Manager 下载 Android 2.3.3 的 SDK 失败，总是报错 `https://dl-ssl.google.com/` 无法访问。估计是被墙了。

解决方法，当然是在 `/etc/hosts` 中添加主机记录（Windows 下这个文件位于 `%SYSTEMROOT%\system32\drivers\etc\hosts`）：

        203.208.46.146 www.google.com
        74.125.113.121 developer.android.com
        203.208.46.146 dl.google.com
        203.208.46.146 dl-ssl.google.com

同时，在 Android SDK Manager 工具的 `Tools -> Options.. -> Others` 中，勾选上 `Force https://... sources to be fetched using http://...`，强制使用 http 下载。

通过以上设置，即可解决。
