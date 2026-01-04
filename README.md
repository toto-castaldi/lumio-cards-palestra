---
lumio_format_version: 1
description: "Flashcard per personal Trainer: contiene esercizi da svolgere in palestra"
---

# Lumio Cards - Palestra

Deck di flashcard per **Personal Trainer** e appassionati di fitness. Ogni carta contiene un esercizio con descrizione, muscoli coinvolti, esecuzione corretta ed errori da evitare.

[![Lumio](https://img.shields.io/badge/Lumio-Deck-blue)](https://lumio.toto-castaldi.com)
[![License: CC0](https://img.shields.io/badge/License-CC0-green)](https://creativecommons.org/publicdomain/zero/1.0/)
[![Cards](https://img.shields.io/badge/Cards-4-orange)](./cards)

## Contenuto

Questo deck copre esercizi per:

| Categoria | Esempi |
|-----------|--------|
| Gambe | Affondi, Squat, Leg Press |
| Petto | Panca piana, Croci, Push-up |
| Schiena | Stacco, Rematore, Lat machine |
| Spalle | Lento avanti, Alzate laterali |
| Braccia | Curl, French press, Dip |
| Core | Plank, Crunch, Russian twist |

## Come Usare

### Con Lumio (Consigliato)

1. Crea un account su [Lumio](https://lumio.toto-castaldi.com)
2. Aggiungi questo repository come deck
3. Studia le card con il sistema di ripetizione spaziata

### Standalone

Puoi navigare le carte direttamente nella cartella [`/cards`](./cards). Ogni file `.md` è una flashcard autonoma.

## Struttura Repository

```
lumio-cards-palestra/
├── README.md           # Questo file
├── CLAUDE.md           # Istruzioni per AI assistant
├── cards/              # Flashcard degli esercizi
│   └── *.md
└── assets/             # Immagini degli esercizi
    └── *.png
```

## Contribuire

Le PR sono benvenute! Per contribuire:

### Creare una Nuova Card

1. Crea un file in `cards/nome-esercizio.md`
2. Usa questo template:

```yaml
---
title: "Nome Esercizio (English Name)"
tags:
  - muscolo-principale
  - tipo-esercizio
  - palestra
difficulty: 2
language: it
---
```

3. Struttura il contenuto con: Immagine, Descrizione, Muscoli, Esecuzione, Errori, Riferimenti

### Requisiti

- `title` e almeno un `tag` ([formato card](https://github.com/toto-castaldi/lumio/blob/v0.6.1/docs/CARD-FORMAT-SPEC.md))
- Contenuto chiaro e verificato
- Immagini in `/assets/` con percorsi relativi (`../assets/file.png`)
- **Riferimenti obbligatori** in fondo a ogni card

### Tag Standard

**Muscoli:** `gambe`, `glutei`, `quadricipiti`, `pettorali`, `dorsali`, `spalle`, `bicipiti`, `tricipiti`, `addominali`, `core`

**Tipo:** `corpo-libero`, `bilanciere`, `manubri`, `macchine`, `cavi`, `funzionale`, `cardio`

## Licenza

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

Questo lavoro è rilasciato nel **Pubblico Dominio** con licenza [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).

Puoi copiare, modificare, distribuire e utilizzare il materiale per qualsiasi scopo, anche commerciale, senza chiedere permesso.

## Disclaimer

Le informazioni contenute in queste carte sono a scopo educativo. Prima di eseguire qualsiasi esercizio:

- Consulta un medico se hai condizioni di salute
- Chiedi a un personal trainer qualificato per la corretta esecuzione
- Ascolta il tuo corpo e non forzare mai oltre i tuoi limiti

## AI Assistant

Questo deck può essere creato/modificato con l'aiuto di Claude o altri AI. Prompt suggerito:

```
Leggi CLAUDE.md per le istruzioni.
Aiutami a creare una nuova card sull'esercizio [NOME ESERCIZIO].
```

Le informazioni nelle carte provengono da ricerche web o conoscenze AI. Ogni carta include i riferimenti alle fonti utilizzate.

---

*Creato con [Lumio](https://github.com/toto-castaldi/lumio)*
