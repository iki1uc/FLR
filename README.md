# FLR – Functional Layer Record

## Öffentlicher Zweck
FLR bildet die öffentliche Meta‑Ebene der Trinity‑Struktur.  
Es dient als sichtbarer Layer zur Dokumentation von Positionen, Items und Lage‑Informationen innerhalb der Public‑Umgebung.

## Argumenteria‑Rahmen
FLR folgt dem Argumenteria‑Prinzip:
1. Klarheit – eindeutige Meta‑Ebene.
2. Struktur – geordnete Darstellung von Layer‑Informationen.
3. Neutralität – keine internen Mechanismen oder Systemdetails.
4. Nachvollziehbarkeit – klarer Zweck und klare Funktion.
5. Integrität – konsistente Außendarstellung.

## 7SINN‑Relevanz
FLR erfüllt die 7SINN‑Kriterien:
1. Verständlichkeit – FLR zeigt Meta‑Informationen klar und nachvollziehbar.
2. Orientierung – dient als strukturierende Übersichtsebene.
3. Nutzen – erleichtert die Zuordnung öffentlicher Daten.
4. Struktur – ordnet Meta‑Elemente und Lage‑Bezüge.
5. Neutralität – bleibt frei von Systeminternas.
6. Integrität – wahrt die Logik der Public‑Ebene.
7. Nachvollziehbarkeit – klare, stabile Darstellung.

## Modulbeschreibung
Dieses Repository stellt die öffentliche FLR‑Ebene dar.  
Es dokumentiert Meta‑Informationen wie Positionen, Items und Lage‑Bezüge innerhalb der Trinity‑Public‑Struktur, ohne interne Abläufe offenzulegen.

## FLR‑CUBE (Public‑Darstellung)
FLR nutzt eine öffentliche Cube‑Struktur, um Meta‑Informationen sichtbar zu machen.  
Diese Darstellung ist neutral gehalten und zeigt nur die öffentlich freigegebenen Felder.

### Beispiel eines FLR‑CUBE (Public‑Version)

```json
{
  "id": "FLR1",
  "info": {},
  "meta": {
    "layer": 1,
    "public": true
  },
  "lage": {
    "pos12": 0,
    "pos4": 0
  },
  "item": {
    "name": "Public-Item",
    "version": "1.0",
    "active": false
  },
  "home": {
    "active": null,
    "pool6": [],
    "pool12": []
  }
}
