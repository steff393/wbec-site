---
layout: default
title: Widerruf
nav_order: 11
---

# Widerrufsrecht und Muster-Widerrufsformular

## Widerrufsrecht für Verbraucher  
(Verbraucher ist jede natürliche Person, die ein Rechtsgeschäft zu Zwecken abschließt, die überwiegend weder ihrer gewerblichen noch ihrer selbstständigen beruflichen Tätigkeit zugerechnet werden können.)

## Widerrufsbelehrung
### Widerrufsrecht
Sie haben das Recht, binnen vierzehn Tagen ohne Angabe von Gründen diesen Vertrag zu widerrufen.  
Die Widerrufsfrist beträgt vierzehn Tage ab dem Tag an dem Sie oder ein von Ihnen benannter Dritter, der nicht der Beförderer ist, die Waren in Besitz genommen haben bzw. hat.  

Um Ihr Widerrufsrecht auszuüben, müssen Sie uns (Ingenieurbüro Stefan Ferstl, Hasenweg 7, 92339 Beilngries, E-Mail: wbec393@gmail.com) mittels einer eindeutigen Erklärung (z.B. ein mit der Post versandter Brief oder E-Mail) über Ihren Entschluss, diesen Vertrag zu widerrufen, informieren. Sie können dafür das beigefügte Musterwiderrufsformular verwenden, das jedoch nicht vorgeschrieben ist.

Zur Wahrung der Widerrufsfrist reicht es aus, dass Sie die Mitteilung über die Ausübung des Widerrufsrechts vor Ablauf der Widerrufsfrist absenden.

### Folgen des Widerrufs
Wenn Sie diesen Vertrag widerrufen, haben wir Ihnen alle Zahlungen, die wir von Ihnen erhalten haben, einschließlich der Lieferkosten (mit Ausnahme der zusätzlichen Kosten, die sich daraus ergeben, dass Sie eine andere Art der Lieferung als die von uns angebotene, günstigste Standardlieferung gewählt haben), unverzüglich und spätestens binnen vierzehn Tagen ab dem Tag zurückzuzahlen, an dem die Mitteilung über Ihren Widerruf dieses Vertrags bei uns eingegangen ist. Für diese Rückzahlung verwenden wir dasselbe Zahlungsmittel, das Sie bei der ursprünglichen Transaktion eingesetzt haben, es sei denn, mit Ihnen wurde ausdrücklich etwas anderes vereinbart; in keinem Fall werden Ihnen wegen dieser Rückzahlung Entgelte berechnet.

Wir können die Rückzahlung verweigern, bis wir die Waren wieder zurückerhalten haben oder bis Sie den Nachweis erbracht haben, dass Sie die Waren zurückgesandt haben, je nachdem, welches der frühere Zeitpunkt ist.

Sie haben die Waren unverzüglich und in jedem Fall spätestens binnen vierzehn Tagen ab dem Tag, an dem Sie uns über den Widerruf dieses Vertrags unterrichten, an uns zurückzusenden oder zu übergeben. Die Frist ist gewahrt, wenn Sie die Waren vor Ablauf der Frist von vierzehn Tagen absenden.

Sie tragen die unmittelbaren Kosten der Rücksendung der Waren in Höhe von 5,49 EUR.

Sie müssen für einen etwaigen Wertverlust der Waren nur aufkommen, wenn dieser Wertverlust auf einen zur Prüfung der Beschaffenheit, Eigenschaften und Funktionsweise der Waren nicht notwendigen Umgang mit ihnen zurückzuführen ist.

## Muster-Widerrufsformular
(Wenn Sie den Vertrag widerrufen wollen, dann füllen Sie bitte dieses Formular aus und senden Sie es zurück.)

- An Ingenieurbüro Stefan Ferstl, Hasenweg 7, 92339 Beilngries, E-Mail: wbec393@gmail.com :

- Hiermit widerrufe(n) ich/ wir (\*) den von mir/ uns (\*) abgeschlossenen Vertrag über den Kauf der folgenden Waren (\*)/
  die Erbringung der folgenden Dienstleistung (\*)

- Bestellt am (\*)/ erhalten am (\*)

- Name des/ der Verbraucher(s)
- Anschrift des/ der Verbraucher(s)
- Unterschrift des/ der Verbraucher(s) (nur bei Mitteilung auf Papier)
- Datum

(\*) Unzutreffendes streichen.

## Widerruf erklären

<style>
  form.widerruf{max-width:600px}
  form.widerruf label{display:block;margin-top:1em}
  form.widerruf input,form.widerruf textarea{
    width:100%;padding:8px;box-sizing:border-box;font-size:1em}
  form.widerruf .hp{position:absolute;left:-9999px}
  form.widerruf button{margin-top:1.5em;padding:12px 20px;background:#b00;
    color:#fff;border:0;border-radius:4px;font-weight:bold;
    cursor:pointer;font-size:1em}
  #ok,#err{margin-top:1em;padding:1em;border-radius:4px;max-width:600px}
  #ok{background:#e6ffe6;border:1px solid #6c6}
  #err{background:#ffe6e6;border:1px solid #c66}
</style>

<p>Hiermit widerrufe ich den von mir abgeschlossenen Vertrag über den Kauf der folgenden Ware:</p>

<form id="f" class="widerruf">
  <label>Name<input name="name" required></label>
  <label>E-Mail (für die Eingangsbestätigung)
    <input type="email" name="email" required></label>
  <label>Vertrag / bestellte Ware
    (z.&nbsp;B. Bestellnummer, Modell, Bestelldatum)
    <textarea name="vertrag" rows="3" required></textarea></label>

  <label class="hp">Bitte leer lassen<input name="website" tabindex="-1" autocomplete="off"></label>
  <button type="submit">Widerruf bestätigen</button>
</form>

<div id="ok" hidden>Ihr Widerruf wurde übermittelt. Sie erhalten in Kürze eine Bestätigung per E-Mail.</div>
<div id="err" hidden>Übermittlung fehlgeschlagen. Bitte später erneut versuchen oder formlos per E-Mail an
     <a href="mailto:wbec393@gmail.com">wbec393@gmail.com</a> widerrufen.</div>

<script>
const ENDPOINT = "https://ferstl.site/widerruf";
document.getElementById("f").addEventListener("submit", async e => {
  e.preventDefault();
  const data = Object.fromEntries(new FormData(e.target));
  try {
    const r = await fetch(ENDPOINT, {
      method:"POST",
      headers:{"Content-Type":"application/json"},
      body: JSON.stringify(data)
    });
    if(!r.ok) throw new Error(r.status);
    e.target.hidden = true;
    document.getElementById("ok").hidden = false;
  } catch {
    document.getElementById("err").hidden = false;
  }
});
</script>
