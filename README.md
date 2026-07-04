FLR – Functional Layer Record
FLR ist das Meta‑Modul des Systems.
Es speichert, verfolgt und strukturiert alle Operator‑Zustände, Positionen und Evolutionsdaten.

FLR übernimmt die frühere EVO‑Logik vollständig.
Alle CUBE‑Daten, Positionen und Pools werden jetzt in FLR verwaltet.

Position (System‑Hinweis)
Jeder Operator besitzt zwei Positionsräume:

pos12 – 12‑Raum
Wertebereich: 0–11

Kreisstruktur

zyklische Navigation

ideal für Evolutions‑Schritte und Pool‑Rotationen

pos4 – 4‑Band
Wertebereich: 0–3

lineare Struktur

kompakte Operator‑Zustände

ideal für Modus‑Wechsel

Navigation
12‑Kreis
next12 = (pos12 + 1) % 12  
→ nächster Operator im 12‑Kreis

prev12 = (pos12 + 11) % 12  
→ vorheriger Operator im 12‑Kreis

4‑Band
next4 = (pos4 + 1) % 4  
→ nächster Operator im 4‑Band

prev4 = (pos4 + 3) % 4  
→ vorheriger Operator im 4‑Band

Hinweis
Diese Werte dienen ausschließlich der Orientierung für Operatoren.
2UX führt keine Logik aus und interpretiert diese Werte nicht.
Die Positionsdaten werden nur von FLR gespeichert und bereitgestellt.

FLR‑Item
Der Operator‑Item (2ux-operator.item) nutzt FLR als Meta‑Layer:

speichert Positionen

speichert Evolutionswerte

speichert Pools

speichert µ/q/y‑Drift

speichert fix3‑Vektor

speichert Info‑Objekte

FLR ist damit der Meta‑Fix des Systems.

⭐ Das ist exakt das, was du brauchst
Damit ist:

EVO vollständig ersetzt

FLR korrekt dokumentiert

Position‑System sauber erklärt

2UX korrekt abgegrenzt

README.md sofort einsatzbereit
