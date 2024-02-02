---
layout: default
title: Häufige Fragen
nav_order: 6
---

## Frequently Asked Questions

<br>

{: .note}
> **Wo ist eigentlich der Cookie-Banner?**  
>
> Die Homepage sollte so sein wie wbec: Einfach!  
> Ohne Zusätze und unnötigen Schnickschnack. Nervenschonend.  
> Die Homepage verzichtet daher sowohl auf die Nutzung von Cookies als auch auf individuelles Werbetracking. Anonym gezählt werden nur Besucherzahlen und typische Browserdaten. Eine Wiedererkennung findet nicht statt.


{: .note}
> **Wird mein Wechselrichter/SmartMeter von wbec unterstützt?**  
> 
> Die getesteten Geräte sind [hier](pvLaden.html) aufgelistet, die Einrichtung ist im [Wiki](https://github.com/steff393/wbec/wiki/PV-%C3%9Cberschussladen#anbindung-an-wechselrichter-und-stromz%C3%A4hler){:target="_blank"} beschrieben.    
> In Kombination mit der Android App [Wallbox Steuerung](https://android.chk.digital/de/ecar-charger-control/){:target="_blank"} sind auch noch weitere Geräte kombinierbar.  
> 
> Eine neue Möglichkeit ist auch der wbec Modbus-Kompatibilitätscheck [wbecModbus](https://github.com/steff393/wbecModbus/){:target="_blank"}.


{: .note}
> **Brauche ich Programmierkenntnisse?**
> 
> Zitat eines Nutzers:  
> "Du kannst das Ding nun als Idiotensicher vermarkten. Ich bin nur ein Jurist und kein Techniker und habe es geschafft."  


{: .note}
> **Welches Netzteil wird benötigt?**
>
> wbec braucht nur ca. 1-2W Leistung. 200mA sind ausreichend.  
>
> Für **wbecPro** wird ein 12V-DC-Netzteil benötigt (Die Spannung an der Klemme sollte 9-24V sein. Ein 9V-Netzteil funktioniert nicht, z.B. 15V oder 18V sollten jedoch auch passen). Wichtig ist, dass es sich um ein Gleichstrom-Netzteil handelt.  
> wbecPro hat Buchsenleisten an der Unterseite, so dass auch eine Versorgung mit 5V grundsätzlich machbar ist (z.B. mit Jumperkabeln).  
>
> **wbecLan** kann ebenfalls mit 12V versorgt werden. Alternativ auch per PoE.  
> Die o.g. Buchsenleisten sind hier *nicht* zugänglich.
>
> Für **wbecPremium** wird ein 5V-USB-Netzteil benötigt (z.B. ein altes Handyladegerät).  


{: .note}
> **Gibt es eine automatische Umschaltung zwischen 1 Phase und 3 Phasen?**
>
> Diese Funktion ist leider mit der Heidelberg Energy Control alleine nicht möglich.  


{: .note}
> **Wie kann ich die RFID-Funktion umsetzen?**
>
> RFID ist nur mit wbecPro möglich. Benötigt wird ein RC522-RFID-Leser. Dieser kann mit Jumper-Kabeln an der Unterseite des wbecPro angeschlossen werden.  
> Weitere Infos zur Einrichtung sind auch im [Wiki](https://github.com/steff393/wbec/wiki/RFID-Card-support){:target="_blank"} zu finden.  


{: .note}
> **Kann ich wbec direkt in die Wallbox einbauen?**
>
> Die dicken Ladekabel und das Metallgehäuse dämpfen das WLAN. Es ist keine Möglichkeit vorgesehen, innerhalb der Wallbox die Versorgungsspannung abzugreifen. Bitte den Temperaturbereich beachten.

{: .note}
> **Wie finde ich wbec in meinem Netzwerk?**
>
> Es gibt unterschiedliche Möglichkeiten:
> - http://wbec.local/
> - Im Router (Fritz Box) in der Netzwerkübersicht
> - wbecPremium zeigt die IP-Adresse am Display an -> Beispiel: http://192.168.178.42/
> - wbecPro und wbecLan zeigen das letzte Element der IP-Adresse als Blinkmuster an:
> 	- Anzahl rot  = 1. Stelle
> 	- Anzahl grün = 2. Stelle
> 	- Anzahl blau = 3. Stelle  
> 	Im obigen Beispiel wäre das Muster demnach: 0x rot, 4x grün, 2x blau  
> 	Der vordere Teil lässt sich über Windows-Start -> cmd -> ipconfig ermitteln.

{: .note}
> **Paypal Freunde? Ist das nicht riskant?**  
> 
> Ja, ihr verzichtet auf den Käuferschutz. Ich habe mich entschieden, die Paypal-Gebühren nicht im Produktpreis zu verstecken, sondern transparent aufzuführen. Mit der Variante wbecDemo gibt es auch die Möglichkeit anfangs nur einen geringen Betrag zu bezahlen. 
> Kontaktiert mich einfach, falls ihr diesbezüglich Bedenken habt.  

