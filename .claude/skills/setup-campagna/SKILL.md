---
name: setup-campagna
description: >
  Bootstrap di Vecna: Eve of Ruin prima della Sessione 01. Il party è fatto di PG delle campagne
  precedenti del ciclo (Curse of Strahd, Dragon Heist, Shadow of the Dragon Queen): la skill li
  recupera dai repo di provenienza, intervista il DM e genera contesto, party, PNG, rapporti.
  Usa questa skill quando il DM dice "/setup-campagna", "inizia la campagna", "i giocatori hanno
  scelto i PG", "prepara il party di Vecna". Da eseguire una sola volta. NON usare a campagna
  avviata — per quello usa /aggiorna-sessione.
---

# Bootstrap Campagna — /setup-campagna

Esegui le istruzioni complete di `ai/agents/00-campaign-setup.agent.md` **nella conversazione
principale**, non come sub-agente: lo Step 2 è un'intervista al DM e un sub-agente non può fare
domande.

## Ordine

1. **Leggi le fonti** (Step 1 dell'agente): il libro, `fonti/campagna/filo-narrativo-multiverso.md`
   e i PG candidati nei repo sorelle (`../dragon-heist-dm`, `../shadow-of-the-dragon-queen-dm`;
   *Curse of Strahd* non ha repo, i PG li fornisce il DM).
2. **Intervista il DM** con tutte le domande dello Step 2 in un unico messaggio. Aspetta le risposte.
3. **Genera i file** (Step 3-7): background in `fonti/personaggi/`, poi `contesto.md`, `party.md`,
   `png-incontrati.md`, `rapporti.md`, aggiunte a `glossario.md`, `INDEX.md`, `QUICK_REF.md`.
4. **Mostra il riepilogo** della *Verifica Finale* con i `[TODO]` rimasti aperti.
5. **Proponi il commit** dei file generati (non fare push senza conferma).

## Regole

- Non piantare semi nuovi del Culto di Vecna: in questa campagna si raccolgono quelli delle
  campagne precedenti, e conta solo ciò che è stato **giocato davvero**, non ciò che era previsto.
- I repo delle campagne precedenti sono sola lettura.

Prossimo passo dopo il setup: `/prep-sessione` per la Sessione 01.
