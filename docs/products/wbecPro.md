---
layout: default
title: wbecPro
parent: Produkte
nav_order: 1
---

wbecPro ist die Standardversion mit WLAN.  

Es wird einfach mittels Schraubklemmen mit dem Modbus-Anschluss der Wallbox verbunden. Zusätzlich wird ein normales 12V-DC-Netzteil benötigt.

Um die Wallbox per WLAN zu erreichen, müsst ihr nur noch die Schalter in der Wallbox richtig einstellen (s. Anleitung) und eure WLAN-Zugangsdaten eintragen.

{: .note-title }
> Auslaufmodell
>
> Beim bisherigen wbecPro ist der Speicher (4MB) bereits zu 99,1% gefüllt (Stand Firmware 1.5.4). Dies begrenzt die zukünftige Erweiterbarkeit. Das neue [wbecProS3](products\wbecProS3.html) bietet nun doppelt so viel Flashspeicher (8MB) bei gleicher Funktionalität. 

<center>
{% assign name = "wbecPro.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  

{% assign name = "modbus.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
</center>  

|Technische Daten             |wbecPro          |
|:----------------------------|:----------------|
|Grundfunktionen              | ja              |
|Web-Interface                | ja              |
|PV-Überschussladen           | möglich         |
|Anbindung powerfox poweropti | möglich         |
|Touch-Display                | nein            |
|RFID-Leser                   | möglich (extern)|
|Flashspeicher                | 4MB             |
|RAM                          | 520kB SRAM      |
|künftige Erweiterbarkeit     | begrenzt        |
|zulässiger Temperaturbereich | 0°C bis 60°C    |
|Spannungsversorgung          | 12V (9-24V)     |
|Abmessungen (BxTxH)          | 58 x 24 x 12mm  |
