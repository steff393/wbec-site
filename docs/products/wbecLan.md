---
layout: default
title: wbecLan
parent: Produkte
nav_order: 3
---

Mit der Ethernet-Variante wbecLan ist jetzt echtes **Plug & Play** *ohne jede Konfiguration* möglich. wbecLan wird mit zwei Adern an die Heidelberg angeschlossen und kann per Netzwerkkabel (PoE) versorgt werden. Sekunden später kann man die Wallbox bereits steuern.  
WLAN ist weiterhin möglich, wird aber nicht mehr benötigt und kann deaktiviert werden.  

Sollte kein Power-over-Ethernet (PoE) zur Verfügung stehen kann man entweder einen PoE-Injektor nutzen oder einfach genauso wie bei wbecPro ein 12V-DC-Netzteil anschließen.

wbecLanS3 ist der Nachfolger des beliebten wbecLan. Es bietet doppelt so viel Flashspeicher (8MB) bei gleicher Funktionalität.  

<center>
{% assign name = "wbecLan.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
</center> 

|Technische Daten             |wbecLan          |wbecLanS3        |
|:----------------------------|:----------------|:----------------|
|Grundfunktionen              | ja              | ja              |
|Web-Interface                | ja              | ja              |
|PV-Überschussladen           | möglich         | möglich         |
|Dynamischer Tarif (*)        | nein            | nein            |
|§14a EnWG (*)                | möglich (mit wbecRse)| möglich (mit wbecRse) |
|Push-Benachrichtigung ntfy.sh| nein            | nein            |
|Anbindung powerfox poweropti | nein            | nein            |
|Touch-Display                | nein            | nein            |
|RFID-Leser                   | nein            | nein            |
|Flashspeicher                | 4MB             | **8MB (!)**     |
|RAM                          | 520kb SRAM      | 520kB SRAM      |
|künftige Erweiterbarkeit     | begrenzt        | begrenzt        |
|zulässiger Temperaturbereich | 0°C bis 60°C    | 0°C bis 60°C    |
|Spannungsversorgung          | PoE oder 12V    | PoE oder 12V    |
|Abmessungen (BxTxH)          | 98 x 24 x 20mm  | 98 x 24 x 20mm  |

(*) gegen gesonderte Aktivierung  
