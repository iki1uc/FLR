# FLR – Functional Layer Record  
Meta‑Layer für Operatoren, Positionen und 12‑CUBE‑Evolutionsdaten

FLR ist der zentrale Meta‑Speicher des Systems.  
Es verwaltet Operator‑Items, Lage‑Daten, Evolutionswerte und Pool‑Strukturen.  
FLR ersetzt die frühere EVO‑LIVE‑Struktur, ohne sie zu zerstören:  
EVO bleibt kompatibel, FLR erweitert das System.

---

## FLR‑CUBE (12‑System)

FLR erzeugt 12 Meta‑Cubes:

- `FLR1` bis `FLR12`
- jeder Cube besitzt eigene Evolutions‑ und Lage‑Daten
- kompatibel mit alten EVO‑Cubes (`EVO1` bis `EVO12`)

### Struktur eines FLR‑CUBE

```json
{
  "id": "FLR1",
  "info": {},
  "evo": 0,
  "eich": 0,
  "gen": 0,
  "fix3": [0, 0, 0],
  "µ": 1,
  "q": 0,
  "y": 0,
  "lage": {
    "pos12": 0,
    "pos4": 0
  },
  "item": {
    "name": "2UX‑Operator",
    "version": "1.0",
    "active": false
  },
  "home": {
    "active": null,
    "pool6": [],
    "pool12": [],
    "pool24": [],
    "pool48": []
  }
}
