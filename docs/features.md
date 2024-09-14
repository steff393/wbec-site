---
layout: default
title: Neue Funktionen
nav_order: 4
---

## Neue Funktionen

### September 2024: GoodWe + SunGrow
Seit Version x.5.3 werden nun auch Wechselrichter von GoodWe (inkl. Batterieleistung) und SunGrow unterstützt.  
<br><br>

### April 2024: §14a EnWG
Mit der neuen Version x.5.2 ist nun die "[§14a EnWG Konformität](https://steff393.github.io/wbec-site/docs/enwg.html)" aktivierbar. Hiermit lassen sich attraktive Rabatte auf die Netzentgelte erzielen.   
<br><br>

### März 2024: SAX Heimspeicher + Victron
Der SAX Heimspeicher kann nun ausgelesen werden und für das PV-Überschussladen genutzt werden. Genutzt werden Bezug/Einspeisung sowie die Batterieleistung.  
Bei Victron-Systemen kann nun ebenfalls die Batterieleistung berücksichtigt werden.  
<br><br>

### Januar 2024: wbecConnect
Auch die neuen "connect"-Modelle von Heidelberg Amperfied können jetzt via Modbus-TCP mit wbec betrieben werden => wbecConnect  
Wallbox connect.home  
Wallbox connect.business  
Wallbox connect.solar  

Sprecht mich einfach an: [wbec393@gmail.com](mailto:wbec393@gmail.com)
<br><br>

### September 2023: Zeitbasierte Steuerung
Mittels http://wbec.local/time.html können Vorgaben zu Start- und Endzeit gemacht werden. Außerdem kann die Energiemenge pro Ladevorgang begrenzt werden. Weitere Infos s. [hier](https://github.com/steff393/wbec/issues/52)  
<center>
{% assign name = "chargeTime.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
</center> 
<br><br>

### Juni 2023: Einbindung in Home Assistant per Script
Vielen Dank an [BenniG82](https://github.com/BenniG82)! Weitere Infos s. [hier](https://github.com/steff393/wbec/pull/81)  
![homeAssistant](https://user-images.githubusercontent.com/6051664/246666850-ae12515e-87fd-4be7-8ba3-52d9499dfa6e.png) 
<br><br>

### Mai 2023: Navigationsleiste im Web Interface
<center>
{% assign name = "navBar.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}"></a>  
</center> 
<br><br>

### Mai 2023: Ladelog
Mittels http://wbec.local/log.html lässt sich eine Übersicht der Ladevorgänge anzeigen. Die Sortierung kann per Klick auf die Spaltenköpfe angepasst werden. Zudem ist ein Export als .csv-Datei möglich.  
<center>
{% assign name = "chargeLog.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
</center> 
<br><br>

### Mai 2023: Konfigurationsseite
Die Parameter können nun einfacher mittels http://wbec.local/cfg.html eingestellt werden. Das Bearbeiten der Datei "cfg.json" mittels http://wbec.local/edit ist natürlich weiterhin möglich.  
<center>
{% assign name = "cfgPage.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
</center> 
<br><br>

### April 2023: IR-Leseköpfe für Stromzähler
Die günstigen IR-Leseköpfe mit Tasmota können nun per HTTP ausgelesen werden. Dies ermöglicht eine einfache und genaue PV-Überschussregelung.  
<br><br>

### Weitere Änderungen
siehe [Release Notes](https://github.com/steff393/wbec/releases)
