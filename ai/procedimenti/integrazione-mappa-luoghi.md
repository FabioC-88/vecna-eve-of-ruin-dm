# Procedimento: Integrazione Mappa Luoghi in Foundry VTT

Questa guida spiega come creare mappe interattive in Foundry VTT per le location della campagna **Vecna: Eve of Ruin**, con pin che linkano direttamente ai **Luoghi Visitati** del compendio.

---

## Obiettivo

Creare Scene (mappe) delle location principali della campagna con pin posizionati sui punti chiave. Ogni pin è un Journal Note che collega a una pagina specifica del compendio "Luoghi Visitati".

*Eve of Ruin* cambia mondo a ogni capitolo: non esiste una mappa del mondo unica, e quasi ogni mappa del libro è una mappa di dungeon o di sito. Una Scene per sito, raggruppate per capitolo.

---

## Prerequisiti

- Foundry VTT con modulo `vecna-eve-of-ruin-dm` attivato nel mondo
- Immagini delle mappe del libro (vedi elenco sotto)
- Compendio "Luoghi Visitati" compilato (generato da `npm run build`)

---

## Step 1: Preparare le Mappe

### Opzione A — Mappe Ufficiali VEoR (Consigliato)

Le mappe sono dentro i capitoli, non in appendice:

| Cap. | Mappe |
|------|-------|
| 1 | 1.1 Neverdeath Catacombs · 1.2 Dolindar Tomb |
| 2 | 2.1 The Sanctum (Sigil) · 2.2 Web's Edge |
| 3 | 3.1 Lambent Zenith · 3.2 Heart of Havock |
| 4 | 4.1 Mount Ironrot Outskirts · 4.2 Ialos · 4.3 Landro |
| 5 | 5.1 Death House |
| 6 | 6.1 Peylon Tree · 6.2 Bittergrass Fen · 6.3 Three Moons Vault · 6.4 Three Moons Vault — Upper Level |
| 7 | 7.1 Isle of Serpents Lagoon · 7.2 Tomb Complex · 7.3 Tomb of Wayward Souls · 7.4 Vortex Bridge Puzzle |
| 8 | 8.1 The Red Belvedere · 8.2 Alabaster Racetrack Stables · 8.3 Scarlet Coliseum · 8.4 Dragon's Pride |
| 9 | 9.1 Pandesmos Outlook |
| 10 | 10.1 Pandesmos Battlefield · 10.2 Hurricane Tower · 10.3 Ruinous Citadel · 10.4 Cliffside Redoubt |
| 11 | 11.1 Vecna's Grasp · 11.2 Torment of Kas · 11.3 Neverwinter Square · 11.4 Arekanz's Donjon · 11.5 Cave of Shattered Reflection |

### Opzione B — Mappe Alternative

Se non hai le mappe ufficiali:
- **D&D Beyond:** asset mappa del libro (se disponibili)
- **Cartography Exchange / Reddit r/dndmaps:** mappe fan dei singoli siti
- **Homebrew:** crea mappe custom usando Inkarnate o simili

---

## Step 2: Creare le Scene in Foundry

1. Apri il tuo mondo Foundry con il modulo attivato
2. Vai in **Scenes** → **Create Scene**
3. Configura:
   - **Name:** `Neverwinter — Catacombe di Neverdeath` (o nome location, come in `campagna/glossario.md`)
   - **Background:** carica l'immagine mappa
   - **Grid Type:** quello della mappa (le mappe di dungeon del libro sono a quadretti)
   - **Visibility:** decidi se visibile ai giocatori subito o solo quando raggiungono la location

---

## Step 3: Aggiungere Note/Pin

1. Nella Scene, attiva il layer **Journal Notes** (icona libro)
2. Clicca **Create Note** e posiziona il pin sulla mappa
3. Per ogni pin, configura:
   - **Journal Entry:** collega alla entry corrispondente nel compendio "Luoghi Visitati"
   - **Icon:** usa un'icona appropriata (cripta, torre, nave, ecc.)
   - **Label:** nome del luogo in italiano

### Location Chiave — esempio (Cap. 1, Neverwinter)

| Location | Tipo | Entry Compendio |
|----------|------|-----------------|
| Villa di Lord Neverember | Residenza | luoghi-visitati/NN-villa-neverember.md |
| Mausoleo Hallix | Cripta | luoghi-visitati/NN-mausoleo-hallix.md |
| Catacombe di Neverdeath | Dungeon | luoghi-visitati/NN-catacombe-neverdeath.md |
| Tomba Dolindar | Cripta | luoghi-visitati/NN-tomba-dolindar.md |

Le tabelle degli altri capitoli si aggiungono quando il party ci arriva: i file in `luoghi-visitati/` li crea l'Agente 7 dopo ogni sessione giocata.

---

## Step 4: Collegare al Compendio

Ogni file in `campagna/luoghi-visitati/` viene compilato nel pack `campagna` del modulo tramite `npm run build`.

Per aggiungere un luogo al compendio:
1. Crea il file `campagna/luoghi-visitati/nome-luogo.md` con il formato standard
2. Esegui `npm run build` per ricompilare i packs
3. In Foundry: **Compendium** → cerca il pack "Note Campagna" → importa nel mondo

---

## Step 5: Organizzare le Scene per Capitolo

Crea una cartella di Scene per capitolo. Struttura consigliata:

```
Cap 1 — Neverwinter/   Catacombe di Neverdeath · Tomba Dolindar
Cap 2 — Sigil/         Il Santuario · Web's Edge
Cap 3 — Mare Astrale/  Lambent Zenith · Heart of Havock
Cap 4 — Eberron/       Mount Ironrot · Ialos · Landro
Cap 5 — Barovia/       Death House
Cap 6 — Krynn/         Albero Peylon · Bittergrass Fen · Three Moons Vault (2 livelli)
Cap 7 — Oerth/         Isle of Serpents · Tomb of Wayward Souls · Vortex Bridge
Cap 8 — Avernus/       Red Belvedere · Scarlet Coliseum · Dragon's Pride
Cap 9-10 — Pandemonio/ Pandesmos Outlook · Battlefield · Hurricane Tower · Ruinous Citadel · Cliffside Redoubt
Cap 11 — Finale/       Vecna's Grasp · Torment of Kas · Neverwinter Square · Arekanz's Donjon · Cave of Shattered Reflection
```

I nomi italiani delle Scene seguono `campagna/glossario.md`: quelli qui sopra ancora in inglese si traducono quando il glossario li fissa.

---

## Note Aggiuntive

- Per i siti con più livelli (Three Moons Vault, Tomb of Wayward Souls) usa una Scene per livello e collega le scale con un pin che apre l'altra Scene
- Le immagini nel file .md sorgente sono in formato webp (path `img/adventure/VEoR/...`) — non sono disponibili nel repository senza il materiale digitale originale

---

> Aggiorna questo file quando aggiungi nuove Scene o cambi la struttura del compendio.
