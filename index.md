---
layout: default
title: Home
nav_order: 1
---

# wbec
{: .text-center}
Heidelberg **W**all**b**ox **E**nergy **C**ontrol  
{: .text-center}

Einfach Überschussladen!
{: .text-center}   

wbec ist die einfachste und schnellste Methode, um dynamisches [PV-Überschussladen](docs/pvLaden.html) mit der Heidelberg Energy Control zu ermöglichen. wbec ist unmittelbar betriebsbereit und muss nicht als komplizierter Linux-Server, Raspberry Pi, o.ä. aufwändig installiert und konfiguriert werden. Man braucht keinen IT-Spezialisten zur Einrichtung. Jeder kann somit eigenen, günstigen Strom tanken.  

Dadurch lassen sich oftmals jährliche Einsparungen von [300 Euro](docs/pvCalc.html) oder mehr erzielen! 

Der Wallbox-Hersteller Heidelberg (jetzt Amperfied) empfiehlt wbec sogar im Blog [Clever laden](https://www.amperfied.de/de/clever-laden/blog/wbec-fuer-heidelberg-wallbox-energy-control-blog/){:target="_blank"}.

{: .new }
> **Coming soon: §14a EnWG**  
>
> Mittels wbec kann die Heidelberg Energy Control künftig konform zu §14a EnWG betrieben werden. Dies ermöglicht eine Reduzierung des Netzentgelts um ca. 150 Euro jährlich, je nach Netzbetreiber. Details folgen ...  
> Schreibt mich gerne dazu an.  

## Benutzeroberfläche
Für wbec ist keine spezielle App erforderlich. Das Webinterface kann mit jedem Browser am PC, Smartphone, Tablet aufgerufen werden und zeigt die wichtigsten Infos und Einstellmöglichkeiten übersichtlich an. Der Ladestrom kann einfach per Schieberegler begrenzt werden.  

<center>
{% assign name = "web.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
</center>  

## Anschluss  
wbec wird einfach mit dem Modbus-RTU-Anschluss der Wallbox verbunden (mit 2 verdrillten Adern eines normalen Netzwerkkabels). Bauliche Veränderungen an der Wallbox sind nicht nötig.  

<center>
{% assign name = "modbus.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ name }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
</center>  

Folgende baugleiche Wallboxen sind ebenfalls kompatibel mit wbec:  
- SENEC Wallbox pro s
- Walther Werke Basic Evo Pro

## Kartenansicht
wbec sorgt seit 2021 bereits bei über 600 Nutzern in ganz Deutschland für optimales Laden! Und täglich werden es mehr. Werde auch du einer davon und sichere dir jetzt dein [wbec-Modul](docs/bestellung.html)!
<center>
{% assign name = "wbecMap.png" %}
{% assign nameBig = "wbecMapLarge.png" %}
<a href="{{ site.url }}{{ site.imgUrl }}{{ nameBig }}"><img src="{{ site.url }}{{ site.imgUrl }}{{ name }}" width="{{ site.imgSize }}"></a>  
<br><small>Klicken für Zoom</small>
</center>  
