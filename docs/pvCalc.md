---
layout: default
title: Rechenbeispiel
nav_order: 7
---
## Rechenbeispiel PV-Überschussladen

### Ausgangslage / Annahmen

|:------------------------------|:----------------------|
|Jährliche Fahrleistung         | 10.000 km             |
|Typischer Verbrauch            | ca. 20 kWh pro 100 km |
|Strompreis bei reinem Netzbezug| 42 ct/kWh ([Durchschnittspreis 1. Halbjahr 2023](https://www.destatis.de/DE/Presse/Pressemitteilungen/2023/09/PD23_388_61243.html){:target="_blank"}) |
|Einspeisevergütung eigene PV   | 10 ct/kWh (z.B. Installation in 2019) |

### Berechnung
Pro Jahr werden also ca. 2000 kWh elektrische Energie verbraucht.  
Dies ergibt Stromkosten für den Netzbezug von **ca. 840 Euro (pro Jahr)**.

Je nach Ladeverhalten und PV-Leistung lassen sich hier deutliche Einsparungen erzielen.

Wenn man es also schafft, den Ladestrom vollständig mit der PV-Anlage abzudecken, ergeben sich Stromkosten für das Laden des Elektroautos von nur noch **200 Euro (pro Jahr)**. In der Praxis wird man aber  
a) nicht immer genügend PV-Leistung haben (z.B. Winter, schlechtes Wetter) oder  
b) das Fahrzeug auch mal z.B. Nachts laden müssen.

### Fazit
In Summe sollte jedoch eine Einsparung von **300 Euro (pro Jahr)** durchaus realistisch sein. Beziehungsweise bei höheren Fahrleistungen, steigenden Strompreisen und fallenden PV-Einspeisevergütungen auch künftig deutlich mehr.

Setzt doch einfach mal eure Werte ein:  

<script type="text/javascript">
function calc() {
	var f = document.querySelector("#fahrleistung").value;
	var v = document.querySelector("#verbrauch").value;
	var p = document.querySelector("#strompreis").value;
	var e = document.querySelector("#einspeisev").value;
	var c = document.querySelector("#prozent").value;
	document.getElementById('ergebnis1').innerHTML = Math.round((p-e) / 100 * v * f * 10); 
	document.getElementById('ergebnis2').innerHTML = Math.round((p-e) / 100 * v * f * 10) * c / 100; 
}
</script>

|:------------------------------|:----------------------|
|Jährliche Fahrleistung         | <input type="number" style="width:50px" onchange="calc()" id="fahrleistung" value=10> Tausend km     |
|Typischer Verbrauch            | <input type="number" style="width:50px" onchange="calc()" id="verbrauch"    value=20> kWh pro 100 km |
|Strompreis bei reinem Netzbezug| <input type="number" style="width:50px" onchange="calc()" id="strompreis"   value=42> ct/kWh         |
|Einspeisevergütung eigene PV   | <input type="number" style="width:50px" onchange="calc()" id="einspeisev"   value=10> ct/kWh         |
|**Mögliche max. Einsparung**   | **<span id="ergebnis1">640</span> Euro (pro Jahr)** |
|**Realistische Einsparung** (<input type="number" style="width:50px" onchange="calc()" id="prozent"   value=50> %)   | **<span id="ergebnis2">320</span> Euro (pro Jahr)** |

