---
layout: default
title: §14a EnWG
nav_order: 5
---
## $14a EnWG Konformität

{: .new }
> **Zusammenfassung**  
>
> - Seit dem 1. Januar 2024 ist es in Deutschland verpflichtend, dass neu installierte E-Auto-Ladestationen ab 4,2 kW durch den Netzbetreiber steuerbar sein müssen.
> - Im Gegenzug gibt es einen jährlichen Rabatt von ca. 150€ - 190€ vom Netzbetreiber (sogenanntes Modul 1).
> - Für Besitzer von vor 2024 installierten Wallboxen besteht eine Wechselmöglichkeit. 
> - Der Rabatt kann auch in Anspruch genommen werden, ohne tätsächlich ein E-Auto zu besitzen. Eine steuerbare, konforme Wallbox ist ausreichend.
> - Mittels wbec erfüllt auch die Heidelberg Energy Control die Kriterien des §14a EnWG (Aktivierung erforderlich*).

### Hintergrund
Um die Netz­sta­bi­lität sicher­zu­stellen, gilt seit dem 1. Januar 2024 die Neure­ge­lung gemäß §14a Ener­gie­wirt­schafts­ge­setz (EnWG) der Bundes­netz­agentur. Diese besagt, dass Netz­an­schlüsse für Ladestationen nicht mehr verwei­gert werden dürfen und die Betreiber gleich­zeitig von redu­zierten Netz­ent­gelten profi­tieren. Im Gegenzug müssen die Betreiber eine Leistungreduzierung (sog. "Dimmung") der Ladestationen während hoher Netz­be­las­tung ermöglichen. Eine Steue­rung ist jedoch nur zur Verhin­de­rung oder Behe­bung einer konkreten Gefähr­dung oder Störung im lokalen Netz zulässig.   

Ab dem 1. Januar 2024 installierte Wallboxen müssen daher zwingend durch den Netzbetreiber steuerbar sein. Bestandsanlagen (vor 2024) können freiwillig durch Antrag beim Netzbetreiber in das neue Modell wechseln und somit ebenfalls von den jährlichen Rabatten profitieren. Alle Netzbetreiber sind seit 2024 verpflichtet dies zu ermöglich.  

### Technische Umsetzung
Das Steuersignal des Netzbetreibers kommt über einen Rundsteuerempfänger (RSE) im Zählerschrank an. Der RSE wird durch den Netzbetreiber installiert, sobald man den Wechsel in das neue Modell beantragt hat. Wichtig ist hierbei, die Variante **"Direktsteuerung"** zu wählen. Ggf. muss durch einen Elektroinstallateur zudem ein Trennrelais verbaut werden.  

Der RSE besitzt einen Schaltkontakt, der je nach Steuersignal entweder offen oder geschlossen ist. Mit diesem Schaltkontakt ist es möglich, zwei Eingänge von [wbecPro](products\wbecPro.html) miteinander zu verbinden. Dadurch erkennt wbecPro, ob eine Reduzierung der Ladeleistung erforderlich ist oder nicht.  

[wbecLan](products\wbecLan.html) und [wbecPremium](products\wbecPremium.html) bieten diese Eingänge **nicht**. Über das Modul [wbecRse](products\wbecRse.html) ist es dennoch möglich, das Signal per WLAN/LAN an wbecLan und wbecPremium oder auch ein weiter entferntes [wbecPro](products\wbecPro.html) zu übertragen.  

wbec sorgt im Falle einer entsprechenden Anforderung dafür, dass die Ladeleistung der angeschlossenen Wallboxen einen Wert von 4,2kW nicht übersteigt. Konkret bedeutet das, dass eine 1-phasig angeschlossene Wallbox mit 16A (3,7kW) laden kann oder eine 3-phasig anschlossene Wallbox mit 6A (4,1kW). Die Ladeleistung weiterer Wallboxen wird auf 0 reduziert.
Nach Beendigung des Steuereingriffs stellt wbec automatisch wieder den vorherigen Strom her.  

*) Die Funktion muss in wbecPro, wbecLan und wbecPremium freigeschalten werden. Hierfür ist ein entsprechender [Aktivierungsschlüssel](docs/bestellung.html) erforderlich. 

### Häufige Fragen

{: .note}
> **Kann es vorkommen, dass mein Fahrzeug nicht mehr geladen wird?**
>
> Die Ladeleistung muss im Falle eines Eingriffs nur auf max. 4,2kW begrenzt werden. Es ist vorgesehen, dass Eingriffe täglich nur ca. 2 Stunden möglich sind. In 2 Stunden lassen sich auch mit reduzierter Leistung trotzdem ca. 50km Reichweite nachladen.  
> Der Netzbetreiber ist verpflichtet, bei häufigen Netzeingriffen die Ausbauplanung des Netzabschnittes zu starten. Somit sollten die Netzeingriffe die *Ultima Ratio* darstellen.  

{: .note}
> **Ich habe schon ein wbec und eine Heidelberg Energy Control. Was brauche ich noch um in das neue Modell zu wechseln?**
>
> - Das wbec muss ein wbecPro sein. Bei wbecLan und wbecPremium ist zusätzlich ein wbecRse erforderlich.  
> - Den EnWG-Aktivierungsschlüssel kannst du [hier bestellen](docs/bestellung.html).  
> - Kläre mit deinem Elektroinstallateur, ob/welche Umbauten am Zählerschrank erforderlich sind.  
> - Du musst bei deinem Netzbetreiber den Wechsel in das neue Modell (Modul 1, Direktsteuerung) beantragen. Eine Rückkehr ins alte Modell ist nicht mehr möglich.   

{: .note}
> **Ich habe nur eine Wallbox, aber noch kein E-Auto. Kann ich trotzdem von den Rabatten profitieren?**
>
> Das EnWG sieht nicht vor, dass an der Ladestation auch tatsächlich ein E-Auto geladen werden muss. Es müssen jedoch die technischen Voraussetzungen geschaffen sein, damit die Leistungreduzierung vorgenommen werden kann.  

{: .note}
> **Mein Netzbetreiber verbaut eine sog. Steuerbox. Ist wbec damit kompatibel?**
>
> Auch die Steuerbox hat (ähnlich wie ein Rundsteuerempfänger) einen Schaltkontakt mit dem das Steuersignal an wbec weitergegeben werden kann.  
