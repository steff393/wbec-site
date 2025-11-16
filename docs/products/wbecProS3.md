---
layout: default
title: wbecProS3
parent: Produkte
nav_order: 2
---

wbecProS3 ist der Nachfolger des beliebten wbecPro.  

Beim bisherigen wbecPro ist der Speicher (4MB) bereits zu 99,1% gefüllt (Stand Firmware 1.5.4). Dies begrenzt die zukünftige Erweiterbarkeit. Das neue wbecProS3 bietet nun doppelt so viel Flashspeicher (8MB) bei gleicher Funktionalität. 

Es wird einfach mittels Schraubklemmen mit dem Modbus-Anschluss der Wallbox verbunden. Zusätzlich wird ein normales 12V-DC-Netzteil benötigt.

Um die Wallbox per WLAN zu erreichen, müsst ihr nur noch die Schalter in der Wallbox richtig einstellen (s. Anleitung) und eure WLAN-Zugangsdaten eintragen.

<center>
{% assign name = "wbecProS3.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  

{% assign name = "modbus.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
</center>  

|Technische Daten             |wbecPro          |wbecProS3        |
|:----------------------------|:----------------|:----------------|
|Grundfunktionen              | ja              | ja              |
|Web-Interface                | ja              | ja              |
|PV-Überschussladen           | möglich         | möglich         |
|Anbindung powerfox poweropti | möglich         | möglich         |
|Touch-Display                | nein            | nein            |
|RFID-Leser                   | möglich (extern)| möglich (extern)|
|Flashspeicher                | **4MB**         | **8MB (!)**     |
|RAM                          | 520kB SRAM      | 520kB SRAM      |
|künftige Erweiterbarkeit     | begrenzt        | begrenzt        |
|zulässiger Temperaturbereich | 0°C bis 60°C    | 0°C bis 60°C    |
|Spannungsversorgung          | 12V (9-24V)     | 12V (9-24V)     |
|Abmessungen (BxTxH)          | 58 x 24 x 12mm  | 58 x 24 x 12mm  |
