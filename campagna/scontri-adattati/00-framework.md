# Framework — Adattamento Scontri

Regole del tavolo valide per **tutti** i capitoli. Vengono da *Shadow of the Dragon Queen*, dove il DM le ha decise e provate al tavolo (settembre-ottobre 2026): per *Eve of Ruin* valgono uguali finché il DM non le cambia, e se cambiano si aggiornano solo qui.

## Perché adattiamo

- **2024 contro 2014:** le schede di *Vecna: Eve of Ruin* sono in formato 2014 (stile *Monsters of the Multiverse*): pochi attacchi, poche Bonus Action e Reaction, quasi nessun effetto sul colpo. I PG con le regole 2024 sono più forti del riferimento con cui il libro è stato scritto.
- **Economia delle azioni:** numero di PG e livelli stanno in `campagna/party.md`. Con più di 4 PG l'azione di un boss solitario si perde tra le iniziative del party: il problema è il numero di azioni, non (solo) il CR.

## Regole fisse

1. **Niente regola Minion.** I gruppi numerosi restano schede classiche, di qualunque dimensione. Per gestirli in fretta al tavolo, le creature con la stessa scheda condividono l'iniziativa: si semplificano i turni, non danni o PF.
2. **Due livelli di nemici nominati:**
   - **Minaccia nominata ma minore** (il boss di una scena, non il motivo per cui il capitolo esiste): una **Bonus Action** e una **Reaction** fisse, nate dalla sua natura, perché non muoia al primo round. Niente Villain Actions.
   - **Boss di fine capitolo o nemesi** (Vecna, Kas): Bonus Action, Reaction e 3 **Villain Actions** (Opener / Control / Ultimate), una per round dopo il turno di un nemico, ciascuna una sola volta a combattimento. Il CR sale solo se il budget lo richiede: la priorità resta l'economia delle azioni, non PF e danni gonfiati.
   - **Come si decide:** «è il motivo per cui questa sessione o questo capitolo esiste, o un ostacolo lungo la strada?». Solo il primo caso merita le Villain Actions.

   Ogni Villain Action ha un breve testo da leggere ai giocatori, che segue le regole dei testi da leggere di `CLAUDE.md`: gesti fisici concreti e dettagli sensoriali, niente costruzioni a contrasto. Il peso del testo scala con l'importanza del nemico. **Non riciclare lo stesso schema tra nemici diversi**: le tre Villain Actions nascono dalla natura del singolo boss, non da «apertura = rinforzi, controllo = area + prono, ultimate = colpo + PF temporanei» con i nomi cambiati.
3. **Lingua:** nomi di creature, azioni e abilità (Actions, Bonus Action, Reaction, Villain Actions, Multiattack) in **inglese**, la terminologia meccanica ufficiale. Tutto ciò che si legge ad alta voce resta in **italiano**, come le note per il DM.
4. **Letalità target: budget in XP della DMG 2024.** Ogni scontro si verifica sommando gli XP **ufficiali** dei mostri (nessun moltiplicatore per il numero) contro questa tabella, **per PG**: si moltiplica per il numero di PG in `campagna/party.md`.

   | Livello | Bassa | Moderata | Alta |
   |:--:|--:|--:|--:|
   | 10 | 1.600 | 2.300 | 3.100 |
   | 11 | 1.900 | 2.900 | 4.100 |
   | 12 | 2.200 | 3.700 | 4.700 |
   | 13 | 2.600 | 4.200 | 5.400 |
   | 14 | 2.900 | 4.900 | 6.200 |
   | 15 | 3.300 | 5.400 | 7.800 |
   | 16 | 3.800 | 6.100 | 9.800 |
   | 17 | 4.500 | 7.200 | 11.700 |
   | 18 | 5.000 | 8.700 | 14.200 |
   | 19 | 5.500 | 10.700 | 17.200 |
   | 20 | 6.400 | 13.200 | 22.000 |

   *I PG di Dragon Heist entrano intorno al 10°; per livelli più bassi vale la stessa tabella della DMG 2024. `[TODO DM: verificare una volta sulla DMG i valori dal 12° in su]`.*

   - **Scontri che contano** (picco della sessione, boss): **Alta**, fino a circa 1,25 × Alta se il party ci arriva riposato.
   - **Scontri di passaggio:** **Moderata**.
   - **Bassa** solo per riempitivi.

   **Perché XP e non somma dei CR.** In *Shadow of the Dragon Queen* (S05, 2026-10-18) uno scontro sotto la Bassa è finito in pochi round con il party quasi illeso: la somma dei CR conta molti nemici deboli come una minaccia seria, ma li ferma un solo incantesimo ad area.
5. **I nemici giocano per vincere.** In ogni scontro che conta:
   - **Ogni capo ha Bonus Action e Reaction:** ufficiali, sergenti e luogotenenti prendono il trattamento «minore» del punto 2 anche se non sono minacce nominate.
   - **Rinforzi a ondate:** almeno un terzo del budget entra al 2°-3° round, da un'altra direzione, così il controllo d'apertura dei PG colpisce solo la prima ondata.
   - **Bersagli intelligenti:** chi ha armi a distanza tira a chi mantiene la concentrazione; dopo il primo incantesimo ad area i gruppi si allargano; chi scopre un terreno pericoloso si ferma e tira invece di attraversarlo.
   - **PF allineati e effetti automatici** secondo la sezione «Allineamento ai numeri 2024» qui sotto. CR e XP restano quelli ufficiali.
   - **Il morale è una valvola, non la regola:** resa o fuga a metà gruppo solo se il tavolo è davvero in difficoltà.

## Cosa NON cambia

- Narrativa, PNG, dialoghi e hook delle dm-notes: questo framework tocca solo schede e regole d'incontro.
- Nessuna mappa o tattica su griglia (gestite da Foundry).

---

## Allineamento ai numeri 2024

Le schede del libro nascono con le regole 2014: le si confronta con i mostri 2024 dello stesso CR e si allinea ciò che resta indietro. **CR e XP ufficiali non cambiano mai**, perché sono il «costo» dello scontro nel budget del punto 4.

**Riferimento:** mediane per CR dell'intero SRD 5.2 (341 mostri), calcolate per *Shadow of the Dragon Queen* il 2026-10-20 sui dati di dnd5eapi.co.

| CR | PF | CA | Danno a round | CD mediana |
|:--:|--:|--:|--:|--:|
| 1/4 | 13 | 12 | 6 | 10-11 |
| 1/2 | 21 | 12 | 8 | 11 |
| 1 | 26 | 13 | 11 | 11 |
| 2 | 45 | 13 | 16 | 12 |
| 3 | 65 | 15 | 24 | 12 |
| 4 | 82 | 15 | 28 | 13 |
| 5 | 105 | 15 | 34 | 14 |
| 6 | 123 | 15 | 41 | 14 |
| 7 | 126 | 17 | 47 | 14 |
| 8 | 136 | 16 | 51 | 15 |
| 9 | 162 | 17 | 60 | 16 |
| 10 | 178 | 18 | 64 | 16 |
| 11 | 199 | 17 | 66 | 17 |
| 12 | 174 | 18 | 90 | 17 |
| 13 | 195 | 17 | 94 | 17 |

*Dal CR 7 in su il campione è piccolo (6-11 mostri per CR, 2 al CR 12): sono indicazioni, non soglie. Dal CR 14 in su il campione SRD è di 1-3 mostri e la regola dei PF non si applica: lì si allineano solo effetti automatici e Bonus Action/Reaction dei capi. Il danno a round è un calcolo grezzo (attacco migliore × numero di attacchi).*

Nel passaggio 5.1 → 5.2 PF, CA, bonus di attacco, CD e tiri salvezza dei mostri sono rimasti uguali; sono cambiati il danno a round dal CR 3 in su, la presenza di Bonus Action e soprattutto gli effetti automatici (condizioni che nel 2014 chiedevano un tiro salvezza e nel 2024 scattano sul colpo).

**Regole.**
1. **PF:** se la scheda è sotto la mediana del suo CR, sale alla mediana; se è sopra, resta. Mai al ribasso. I dadi vita si aggiornano insieme ai PF: la formula, con il modificatore di COS della scheda, deve dare il totale scritto (se nessuna cade esattamente sulla mediana, la più vicina per eccesso).
2. **CA, danno, CD e TS non si toccano.**
3. **Effetti automatici:** un «TS o Prono/Afferrato» da colpo, che nel 2024 sarebbe automatico, lo diventa. Paralisi, Spaventato e simili restano a tiro salvezza.
4. **Capi:** una Bonus Action e una Reaction fisse (punto 5).

Le differenze per ogni creatura si scrivono **solo** in [aggiornamenti-schede.md](aggiornamenti-schede.md), quando si prepara la sessione in cui compare. I PF più alti allungano gli scontri: dopo ogni sessione reale si ricontrolla e, se serve, si corregge il budget (`[TODO DM: verificare]` dove il numero è a giudizio).
