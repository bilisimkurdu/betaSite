---
id: 376
title: Windows 10 Cortana devre dışı bırakma
date: 2018-11-20T22:45:51+00:00
author: Yakup Contarlı
layout: post
guid: http://localhost/bilisimkurdu/?p=376
permalink: /windows-10-cortana-devre-disi-birakma/
ampforwp_custom_content_editor:
  - ""
ampforwp_custom_content_editor_checkbox:
  - null
ampforwp-amp-on-off:
  - default
ampforwp-redirection-on-off:
  - enable
image: /wp-content/uploads/2018/11/59fde5bccfdf4_maxresdefault.jpg
categories:
  - PC
  - Windows
tags:
  - bırakma
  - cortana
  - devre dışı
  - disable
  - windows 10
  - windows 10 cortana
  - windows 10 cortana devre dışı
  - windows 10 cortana devre dışı bırakma
  - windows 10 cortana disable
---
Merhaba Muhterem ziyaretçilerimiz,
  
Bugün Windows 10 Cortana disable (devre dışı bırakacağımızı) nasıl edileceğini anlatacağım. Bilindiği üzere Cortana Microsoft&#8217;un asistan uygulaması olup işlevi yerine getirebilmesi için verilerinizi toparlayıp analiz edilmektedir.

<!--more-->

Cortana&#8217;yi disable ederek gizliliğinizi bir nebzede koruyabilirsiniz.

Windows 10 Pro ve Enterpise

  1. **Başlat ->** **gpedit.msc**
  2.  **Computer Configuration > Administrative Templates > Windows Components > Search yolunu takip ederek **
  3. **Allow Cortana** ayarını bulup çift tıklatınız **disable** ederek bilgisayarınız restart ediniz.

<img class="aligncenter wp-image-341112" src="https://betanews.com/wp-content/uploads/2016/07/GPE.jpg" sizes="(max-width: 640px) 100vw, 640px" srcset="https://betanews.com/wp-content/uploads/2016/07/GPE.jpg 2182w, https://betanews.com/wp-content/uploads/2016/07/GPE-300x227.jpg 300w, https://betanews.com/wp-content/uploads/2016/07/GPE-768x582.jpg 768w, https://betanews.com/wp-content/uploads/2016/07/GPE-600x455.jpg 600w, https://betanews.com/wp-content/uploads/2016/07/GPE-900x682.jpg 900w" alt="GPE" width="640" height="485" />

Windows 10 Home

**Başlat -> Regedit -> HKEY\_LOCAL\_MACHINE\SOFTWARE\Policies\Microsoft\Windows\Windows Search** yolunu takip ediniz.

Windows klasörünün üzerine sağtık ile tıklayarak &#8220;**New->Key&#8221;** yolunu takip ederek &#8220;**Windows Search**&#8221; değerini veriniz.

<img class="aligncenter size-full wp-image-298234" src="https://img.purch.com/o/aHR0cDovL3d3dy5sYXB0b3BtYWcuY29tL2ltYWdlcy93cC9wdXJjaC1hcGkvaW5jb250ZW50LzIwMTYvMDkvc2NyZWVuc2hvdC0oMTA0KV82MzguNzYwODA2OTE2NDM0MDMucG5n" alt="screenshot (104) 638.76080691643403" width="638" height="403" />

**Windows Search** klasörün üzerine sağtık ile **&#8220;DWORD (32-bit) Value&#8221;** ekliyoruz.<img class="aligncenter size-full wp-image-298236" src="https://img.purch.com/o/aHR0cDovL3d3dy5sYXB0b3BtYWcuY29tL2ltYWdlcy93cC9wdXJjaC1hcGkvaW5jb250ZW50LzIwMTYvMDkvc2NyZWVuc2hvdC0oMTA1KV82NzUyODEuMjUucG5n" alt="screenshot (105) 675281.25" width="675" height="281" />

&nbsp;

4. **DWORD ** değeri **&#8220;AllowCortana&#8221;** değeri **&#8220;0&#8221;** olmalıdır. En sonunda bilgisayarı restart ediyoruz.

<img class="aligncenter size-full wp-image-298238" src="https://img.purch.com/o/aHR0cDovL3d3dy5sYXB0b3BtYWcuY29tL2ltYWdlcy93cC9wdXJjaC1hcGkvaW5jb250ZW50LzIwMTYvMDkvc2NyZWVuc2hvdC0oMTA2KV82NzUxNTQuMjg1NzE0Mjg1NzEucG5n" alt="screenshot (106) 675154.28571428571" width="675" height="154" />