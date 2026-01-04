# Istruzioni per Claude - Deck Palestra

## Scopo del Deck

Flashcard per Personal Trainer: esercizi da svolgere in palestra.

## Formato Card Lumio

Ogni card è un file `.md` nella cartella `cards/` con questo frontmatter:

```yaml
---
title: "Nome Esercizio (Nome Inglese)"
tags:
  - tag1
  - tag2
  - palestra
difficulty: 2
language: it
---
```

### Campi Obbligatori
- `title`: nome esercizio in italiano (nome inglese tra parentesi)
- `tags`: minimo 1 tag, minuscolo, senza spazi. Includere sempre `palestra`

### Campi Opzionali
- `difficulty`: 1-5 (default: 3)
- `language`: codice ISO 639-1 (default: "it")

### Tag Comuni
- Muscoli: `gambe`, `glutei`, `quadricipiti`, `pettorali`, `dorsali`, `spalle`, `bicipiti`, `tricipiti`, `addominali`, `core`
- Tipo: `corpo-libero`, `bilanciere`, `manubri`, `macchine`, `cavi`, `funzionale`, `cardio`
- Sempre: `palestra`

## Struttura Contenuto Card

L'ordine delle sezioni deve essere:

1. **Immagine** (prima cosa visibile)
2. **Descrizione** (breve, 2-3 frasi)
3. **Muscoli Coinvolti** (lista puntata con spiegazione ruolo)
4. **Esecuzione** (lista numerata passo-passo)
5. **Varianti** (tabella se applicabile)
6. **Errori Comuni** (lista puntata)
7. **Riferimenti** (sempre in fondo, dopo `---`)

## Immagini

- Cartella: `/assets/`
- Path nella card: `../assets/nome-file.png`
- Fonte preferita: Wikimedia Commons (licenza libera)
- Formato: PNG o SVG

```markdown
## Immagine

![Nome Esercizio](../assets/nome-esercizio.png)
```

## Riferimenti

**OBBLIGATORIO**: Ogni card deve avere una sezione Riferimenti in fondo.

Se uso fonti web:
```markdown
---

### Riferimenti

- [Titolo - Sito](https://url)
- [Titolo - Sito](https://url)
- Immagine: [Wikimedia Commons - Nome](https://url) (Licenza)
```

Se NON uso fonti esterne:
```markdown
---

### Riferimenti

Contenuto creato senza fonti esterne, basato su conoscenze generali.
```

## Naming File

- Nome file: `nome-esercizio.md` (minuscolo, trattini)
- Esempio: `affondo-in-camminata.md`, `panca-piana.md`, `stacco-da-terra.md`

## Esempio Completo

```markdown
---
title: "Nome Esercizio (English Name)"
tags:
  - muscolo1
  - muscolo2
  - tipo
  - palestra
difficulty: 2
language: it
---

## Immagine

![Nome Esercizio](../assets/nome-esercizio.png)

## Descrizione

Breve descrizione dell'esercizio in 2-3 frasi.

## Muscoli Coinvolti

- **Muscolo principale**: ruolo nel movimento
- **Muscolo secondario**: ruolo nel movimento

## Esecuzione

1. Primo passo
2. Secondo passo
3. Terzo passo

## Varianti

| Variante | Effetto |
|----------|---------|
| Variante A | Descrizione |
| Variante B | Descrizione |

## Errori Comuni

- Errore 1
- Errore 2

---

### Riferimenti

- [Fonte 1](https://url)
- [Fonte 2](https://url)
```

## Workflow

1. Utente chiede card su esercizio X
2. Cerco informazioni sul web (WebSearch)
3. Cerco immagine libera su Wikimedia Commons
4. Creo card in `cards/nome-esercizio.md`
5. Immagine in `/assets/` (se disponibile localmente)
6. Riferimenti sempre in fondo
