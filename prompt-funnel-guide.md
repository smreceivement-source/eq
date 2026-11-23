# Prompt per Claude Code: funnel guide gratis + guide a pagamento

Strumenti: **Google Drive** (file), **ManyChat** (DM Instagram), **Systeme.io** (pagine, email, vendita).

Due funnel:
- **A:** Guida Natale (gratis) → Valorizzazione della casa (a pagamento)
- **B:** Percezione dell'immobile in affitto (gratis) → "Case che vendono" (a pagamento)

## Come si usano

1. Crea una cartella vuota sul computer (es. `funnel-guide`) e mettici dentro i 4 PDF.
2. Apri Claude Code in quella cartella.
3. Incolla i prompt **in ordine**, uno alla volta. Ogni prompt salva il suo risultato in un file, così il successivo lo riusa e non si riparte da zero.

Claude Code **scrive tutto** (testi, email, DM, istruzioni passo passo). **Non entra da solo** in Systeme o ManyChat: lì incolli tu i testi. Fa eccezione l'estensione *Claude in Chrome*, se è attiva: con quella può compilare le pagine al posto tuo (vedi il Prompt 6).

---

## PROMPT 0 · Brief del progetto (fallo oggi, 5 minuti)

```
Sto creando due funnel di vendita per le mie guide. Voglio che tu prepari un file
CLAUDE.md in questa cartella con il brief del progetto: lo userai come riferimento
in tutti i passaggi successivi.

Prima leggi i PDF presenti nella cartella e riassumi per ciascuno: titolo, a chi è
rivolto, promessa principale, 5 punti chiave del contenuto.

Poi fammi le domande UNA ALLA VOLTA per completare il brief:
- il mio nome/brand e come voglio essere chiamata
- tono di voce (es. caldo, professionale, ironico) e 2-3 parole che non userei mai
- il mio pubblico Instagram (chi sono, cosa li frena)
- prezzo di ciascuna guida a pagamento e se voglio un prezzo lancio con scadenza
- eventuale order bump (piccolo extra a prezzo basso) per ogni funnel
- le parole chiave per i commenti Instagram (proposta: NATALE e AFFITTO)
- email mittente e nome mittente

Struttura dei funnel da scrivere nel brief:
Funnel A: guida gratis Natale → upsell guida "Valorizzazione della casa"
Funnel B: guida gratis "Migliorare la percezione della location in affitto" →
upsell guida "Case che vendono" (guida operativa per migliorare resa economica e
prenotazioni).
Flusso: commento IG con parola chiave → DM ManyChat con link → pagina Systeme di
iscrizione (email) → pagina offerta con modulo d'ordine + order bump → email di
consegna → 3 email di follow-up per chi non compra.

Alla fine mostrami il CLAUDE.md completo e chiedimi conferma prima di salvarlo.
```

---

## PROMPT 1 · Checklist prima della sessione

```
Usando CLAUDE.md, creami il file 01-checklist.md con tutto quello che devo avere
pronto PRIMA di costruire i funnel, diviso in: account (Systeme, Stripe/PayPal,
Instagram professionale collegato a Pagina Facebook, ManyChat), file, decisioni,
aspetti legali/fiscali minimi per vendere prodotti digitali in Italia (ricevuta,
privacy, consenso email). Per ogni voce: come verificare che è fatta, tempo stimato
e cosa fare se si blocca. Metti in cima le cose che richiedono giorni (es. verifica
Stripe). Poi fammi spuntare le voci una per una chiedendomi a che punto sono.
```

---

## PROMPT 2 · Testi delle pagine Systeme

```
Usando CLAUDE.md e il contenuto dei PDF, scrivi i testi delle pagine Systeme per
ENTRAMBI i funnel e salvali in 02-pagine-funnel-A.md e 02-pagine-funnel-B.md.

Per ogni funnel:
1. Pagina di iscrizione (guida gratis): 3 opzioni di titolo, sottotitolo, 3-4 punti
   "cosa trovi nella guida", testo del bottone, micro-testo privacy sotto il form.
2. Pagina offerta (dopo l'iscrizione): titolo "la guida sta arrivando…", testo
   di vendita breve della guida a pagamento (problema → soluzione → cosa contiene →
   per chi è / per chi non è → prezzo → garanzia se la offro), testo dell'order bump
   (max 2 righe, inizia con "Sì,"), link "No grazie".
3. Pagina di ringraziamento dopo l'acquisto.
4. Testo della pagina di ringraziamento per chi ha preso solo la guida gratis.

Scrivi nel mio tono di voce. Frasi corte, niente promesse non dimostrabili sui
guadagni. Indica tra [parentesi quadre] dove va un'immagine o un mockup.
```

---

## PROMPT 3 · Email automatiche

```
Usando CLAUDE.md, scrivi le email per Systeme per entrambi i funnel e salvale in
03-email.md. Per ogni funnel:
- Email 1 (subito dopo l'iscrizione): consegna della guida gratis con [LINK DRIVE]
  e un accenno alla guida a pagamento.
- Email 2 (+2 giorni): un consiglio pratico di valore + invito alla guida a pagamento.
- Email 3 (+4 giorni): obiezione più comune e risposta + scadenza del prezzo lancio
  (se prevista).
- Email di consegna dopo l'acquisto (con [LINK PRODOTTO]).
Per ognuna: 2 oggetti alternativi, anteprima, corpo, CTA. Max 150 parole.
In fondo al file scrivi la tabella dell'automazione Systeme da creare:
trigger → tag → azione → ritardo, e la regola per togliere dal follow-up chi ha
già comprato.
```

---

## PROMPT 4 · ManyChat + contenuti Instagram

```
Usando CLAUDE.md, prepara tutto per ManyChat e salvalo in 04-manychat-instagram.md.
Per ogni funnel:
1. Automazione "commento con parola chiave": parola chiave + varianti da includere
   (minuscole, con errori comuni), risposta pubblica al commento (3 varianti da
   ruotare), DM con il link alla pagina di iscrizione.
2. Messaggio di follow-up dopo 24 ore se non ha cliccato.
3. Risposta automatica per chi scrive la parola chiave in DM invece che nei commenti.
4. Le istruzioni passo passo per creare l'automazione in ManyChat (quali menu
   cliccare), in modo semplice per chi non l'ha mai usato.
5. Caption del post di lancio + script di un reel di 20-30 secondi che invita a
   commentare la parola chiave.
```

---

## PROMPT 5 · Google Drive

Se Claude ha accesso a Google Drive (connettore attivo):
```
Su Google Drive crea una cartella "Guide - Funnel" con le sottocartelle "Gratis" e
"A pagamento". Carica/sposta lì i PDF delle guide. Imposta le guide GRATIS come
"chiunque abbia il link può visualizzare". Le guide A PAGAMENTO lasciale private.
Poi scrivi i link delle guide gratis in 05-link.md e sostituisci [LINK DRIVE] in
03-email.md con il link giusto per ogni funnel.
```
Se non ha accesso:
```
Spiegami passo passo come caricare le guide su Google Drive e condividere le due
guide gratis con "chiunque abbia il link". Poi chiedimi di incollarti i due link
e sostituisci [LINK DRIVE] in 03-email.md.
```

---

## PROMPT 6 · Costruzione in Systeme (in sessione)

```
Guidami a costruire in Systeme.io il Funnel A, usando i file 02-pagine-funnel-A.md,
03-email.md e 05-link.md. Procedi UN PASSO ALLA VOLTA e aspetta che ti dica "fatto"
prima di passare al successivo:
1. creazione del prodotto digitale e del prezzo (con il file della guida a pagamento)
2. creazione del funnel e delle pagine (iscrizione, offerta con modulo d'ordine e
   order bump, ringraziamento)
3. per ogni pagina: quale testo incollare e in quale blocco
4. tag e automazioni (iscrizione → tag → email 1, poi 2 e 3; acquisto → tag →
   email di consegna, stop follow-up)
5. impostazioni email (mittente, dominio)
Ad ogni passo dimmi esattamente cosa cliccare. Quando il Funnel A è finito, dimmi
come DUPLICARLO per creare il Funnel B e quali elementi cambiare.
```
Se hai l'estensione **Claude in Chrome** attiva, aggiungi in fondo:
`Usa il browser per compilare tu i campi in Systeme mentre io guardo, e fermati prima di salvare o pubblicare.`

---

## PROMPT 7 · Test finale

```
Creami la checklist 07-test.md per testare entrambi i funnel dall'inizio alla fine
come se fossi una cliente: commento IG → DM → iscrizione → email ricevuta (controlla
anche lo spam) → link Drive funzionante → acquisto di prova (Stripe in modalità
test o coupon 100%) → email di consegna → stop del follow-up dopo l'acquisto.
Per ogni punto: cosa deve succedere e, se non succede, le 2-3 cause più probabili e
come risolverle. Poi guidami nel test punto per punto.
```

---

## PROMPT 8 · Dopo una settimana

```
Ti incollo i numeri dei funnel (commenti, DM inviati, click, iscritti, vendite,
aperture e click delle email). Calcola i tassi di conversione per ogni passaggio,
dimmi dov'è il punto debole principale di ciascun funnel e proponimi 3 modifiche
concrete (con il nuovo testo già scritto) da testare la settimana prossima.
```

---

### Ordine consigliato
- **Oggi o stasera:** Prompt 0 → 1 → 2 → 3 → 4 → 5 (tutto il testo è pronto prima della sessione)
- **In sessione (15 minuti):** Prompt 6 → 7
- **Dopo 7 giorni:** Prompt 8
