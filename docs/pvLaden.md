---
layout: default
title: PV-Überschussladen
nav_order: 5
---
## PV-Überschussladen
Dynamisches PV-Überschussladen ist sicherlich die interessanteste Einsatzmöglichkeit für wbec.

### Beschreibung
Strom aus dem Netz wird immer teurer. Im Gegenzug steht jedoch mehr und mehr günstiger, eigener PV-Strom zur Verfügung für den man nur noch niedrige Einspeisevergütungen erhält.  
Was liegt also näher, als das e-Auto möglichst mit Strom aus der Sonne zu betanken?

Die Heidelberg Energy Control stellt dem Fahrzeug normalerweise einen fest eingestellten, maximalen Ladestrom zur Verfügung.  
Mit Hilfe von wbec kann dieser maximale Ladestrom jedoch an die aktuellen Gegebenheiten dynamisch angepasst werden. 

{: .note-title }
> Beispiel
>
> Aktuell erzeugt die PV eine Leistung von 6 kW.  
> Der Hausverbrauch beträgt 0,5 kW.  
> Die Wallbox ist auf 8 A (= 5,5 kW) eingestellt.  
> Es wird folglich weder ins Netz eingespeist, noch Strom aus dem Netz bezogen (idealer Zustand).  
>  
> Nun erhöht sich die PV-Leistung durch mehr Sonnenschein um 3 kW, beträgt also nun 9 kW.  
> Dies führt zunächst zu einer Einspeisung von 3 kW ins Stromnetz, die vom Smartmeter gemessen wird.  
> **wbec** kann nun die Ladeleistung der Wallbox auf 8,5 kW (= 12,3 A) erhöhen.
> In der Folge fließt der zusätzliche PV-Strom nicht mehr ins Netz, sondern ins Auto. Der ideale Zustand ist wieder erreicht.  

Weitere Informationen finden sich auch im [Wiki](https://github.com/steff393/wbec/wiki/PV-%C3%9Cberschussladen) auf Github.  

### Kompatible Wechselrichter per Modbus-TCP
- SolarEdge (z.B. SE7k, SE9k)
- Fronius (z.B. Symo 17.5 + Fronius Smartmeter)
- Kostal mit KSEM (Kostal Smart Energy Meter)
- Kostal ohne KSEM (z.B. Plenticore Plus 10)
- Huawei (z.B. Huawei Sun2000 Wechselrichter mit DTSU 666 Power Meter)
- SMA mit Smartmeter (z.B. Sunny Tripower STP8-10-3AV-40 aus 2021)
- SMA Sunny Home Manager 2.0 (z.B. mit Sunny Tripower 8.0 Smart Energy)
- Victron (z.B. Victron cerbo gx (inkl. Smartmeter Victron EM24 RS485, Wechselrichter Multiplus2 5000), Victron Easy Control GX)
- E3DC
- SAX-Power Heimspeicher (mit EnFluRi-Sensor)
- Goodwe mit Smartmeter und WiFi/LAN-Kit v2 (z.B. GW10KN-ET)
- SunGrow

### Smartmeter (oder Speicher) per HTTP
- Shelly 3EM
- Shelly 3EM Pro
- sonnenBatterie  (z.B. Eco 8.0)
- powerfox poweropti
- IR-Leseköpfe für Stromzähler (z.B. Tasmota, Bitshake, o.ä.)

### Energiemanagementsysteme
- Android-App [Wallbox Steuerung](https://android.chk.digital/de/ecar-charger-control/){:target="_blank"}
- openWB, openWB 2.0 (per MQTT oder als emulierter go-eCharger)
- evcc (per MQTT oder als emulierter go-eCharger)
- Solaranzeige (als emulierter go-eCharger)

### Smart-Home-Systeme
- Home Assistant (per MQTT oder HTTP)
- IP Symcon (per HTTP)
- openHAB (per HTTP)
- Loxone (über virtuelle Ausgangsverbinder)
- ioBroker
- Nodered Redmatic


## Weitere Infos
Die Anbindung ist im Detail im [Wiki](https://github.com/steff393/wbec/wiki/PV-%C3%9Cberschussladen) beschrieben.  

Dein System/Wechselrichter ist nicht genannt? Die Android-App [Wallbox Steuerung](https://android.chk.digital/de/ecar-charger-control/){:target="_blank"} unterstützt sehr viele Wechselrichter, bietet noch mehr Funktionen als wbec alleine und lässt sich sehr einfach gemeinsam mit wbec und der Heidelberg Energy Control nutzen.
