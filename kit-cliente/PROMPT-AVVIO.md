# Prompt da incollare in Claude Code

Copia tutto quello che c'è nel riquadro qui sotto e incollalo in Claude Code, aperto nella cartella `kit-cliente`.

```
Sei il mio assistente per mettere online due funnel di vendita delle mie guide.
Non ho mai usato automazioni: spiegami tutto in modo semplice, in italiano, senza
gergo tecnico. Lavora per STEP. Alla fine di ogni step fermati, riassumi in 3 righe
cosa abbiamo fatto e aspetta che io scriva "ok" prima di passare al successivo.
Salva ogni risultato nella cartella lavoro/ e tieni aggiornato lavoro/stato.md con
lo step attuale, così possiamo riprendere in qualsiasi momento.

IL PROGETTO
Strumenti: Systeme.io PIANO GRATUITO (pagine, email, vendita), ManyChat
(risposte automatiche su Instagram) e, solo se serve, Google Drive.
Le guide sono nella cartella guide/, una per sottocartella:
- Funnel A: guide/1-natale-GRATIS → upsell guide/2-valorizzazione-casa-PAGAMENTO
- Funnel B: guide/3-percezione-affitto-GRATIS → upsell
  guide/4-case-che-vendono-PAGAMENTO (guida operativa per migliorare resa
  economica e prenotazioni di un immobile in affitto)
Percorso del cliente: commenta una parola chiave sotto un post Instagram →
ManyChat gli manda in DM il link → pagina Systeme dove lascia l'email e riceve
la guida gratis → pagina offerta con la guida a pagamento (+ eventuale order
bump) → email di consegna → 3 email di follow-up per chi non compra (e stop
delle email per chi ha comprato).

REGOLE
- Non inventare funzioni di Systeme o ManyChat. Se non sei sicuro che una cosa
  esista nel piano gratuito, dimmelo e fammela verificare nel mio account
  indicandomi dove guardare.
- Niente promesse di guadagno non dimostrabili nei testi.
- Non pubblicare, salvare o pagare nulla al posto mio senza chiedermelo.

GLI STEP

STEP 1. Controllo delle guide
Controlla che in ognuna delle 4 sottocartelle di guide/ ci sia un PDF. Se ne
manca uno, fermati e dimmelo. Leggi i PDF e, per ciascuno, scrivi in
lavoro/01-guide.md: titolo, a chi è rivolta, promessa principale, 5 punti chiave,
numero di pagine e peso del file in MB.

STEP 2. Brief del progetto
Fammi le domande UNA ALLA VOLTA (proponendo tu una risposta di esempio):
nome/brand, tono di voce, pubblico Instagram, prezzo delle 2 guide a pagamento,
prezzo lancio sì/no e scadenza, order bump sì/no (proponimi tu un'idea di extra
per ogni funnel partendo dai PDF), parole chiave per i commenti (proposta:
NATALE e AFFITTO), nome ed email del mittente, partita IVA o no (solo per
ricordarmi cosa scrivere nelle condizioni di vendita).
Salva tutto in CLAUDE.md in questa cartella, così lo rileggi da solo ogni volta.

STEP 3. Verifica del piano gratuito di Systeme e scelta della soluzione più rapida
Guidami ad aprire il mio account Systeme e a verificare, voce per voce, cosa
permette il mio piano: numero di funnel, numero di corsi, regole di automazione o
workflow, numero di tag, se l'editor delle email permette di allegare un file, se
il modulo d'ordine permette order bump e upsell, se Stripe e PayPal sono collegati.
Dimmi esattamente dove cliccare per ogni verifica e annota le mie risposte in
lavoro/03-limiti-systeme.md.
Poi, IN BASE AI LIMITI REALI, scegli il modo più semplice per consegnare le
4 guide, valutando queste opzioni (dalla preferita):
  a) guide a pagamento dentro un corso Systeme (se i corsi bastano)
  b) guida allegata direttamente all'email automatica (se è possibile)
  c) link Google Drive "chiunque abbia il link" dentro l'email (soluzione di
     riserva, la più veloce)
Mostrami una tabella guida → metodo di consegna → perché, con pro e contro, e
fammi scegliere. Se serve Drive, spiegami passo passo come caricare solo i file
necessari e condividerli, poi chiedimi di incollarti i link.
Salva la decisione in lavoro/03-consegna.md.

STEP 4. Checklist degli account
Crea lavoro/04-checklist.md con quello che deve essere pronto prima di costruire:
Systeme (email mittente verificata, Stripe/PayPal collegati), Instagram
professionale collegato a una Pagina Facebook, ManyChat collegato a Instagram,
privacy e condizioni di vendita minime per vendere prodotti digitali in Italia.
Metti in cima le cose che richiedono tempo (es. verifica Stripe). Fammi spuntare
le voci una alla volta e, per ognuna bloccata, dimmi come sbloccarla.

STEP 5. Testi delle pagine
(Se usiamo PROMPT-PAGINE-VENDITA.md, questo step si salta: le pagine complete
le crea quel prompt.)
Per ciascun funnel scrivi in lavoro/05-pagine-A.md e lavoro/05-pagine-B.md:
pagina di iscrizione (3 titoli a scelta, sottotitolo, 3-4 punti "cosa trovi",
bottone, nota privacy), pagina offerta (titolo "la guida sta arrivando…", testo
di vendita breve: problema, soluzione, contenuto, per chi è, prezzo; testo order
bump di 2 righe che inizia con "Sì,"; link "No grazie"), pagina di ringraziamento
dopo l'acquisto. Usa il contenuto vero dei PDF e il mio tono di voce. Indica tra
[parentesi quadre] dove mettere le immagini.

STEP 6. Email
In lavoro/06-email.md, per ciascun funnel: email 1 di consegna della guida gratis
(subito), email 2 di valore (+2 giorni), email 3 con obiezione e scadenza
(+4 giorni), email di consegna dopo l'acquisto. Per ognuna: 2 oggetti, anteprima,
testo (max 150 parole), bottone. Usa il metodo di consegna scelto allo step 3.
In fondo, la tabella delle automazioni da creare (evento → tag → azione →
ritardo), compatibile con i limiti del piano gratuito annotati allo step 3.

STEP 7. ManyChat e Instagram
In lavoro/07-manychat.md, per ciascun funnel: parola chiave e varianti,
3 risposte pubbliche al commento da alternare, DM con il link, follow-up dopo
24 ore per chi non clicca, risposta per chi scrive la parola chiave in DM, e le
istruzioni passo passo per creare l'automazione in ManyChat (piano gratuito: se
una funzione richiede il piano Pro, dimmelo e proponimi l'alternativa gratuita).
Aggiungi la caption del post di lancio e lo script di un reel di 20-30 secondi.

STEP 8. Costruzione in Systeme (lo facciamo in sessione)
Guidami un'azione alla volta, aspettando il mio "fatto": prodotto e prezzo,
funnel A con le sue pagine e i testi presi da lavoro/05-pagine-A.md, modulo
d'ordine e order bump, tag e automazioni da lavoro/06-email.md. Poi spiegami
come DUPLICARE il funnel A per creare il B (dentro il limite di funnel del piano
gratuito) e cosa cambiare. Ad ogni passo dimmi esattamente cosa cliccare.
Se ho attiva l'estensione Claude in Chrome, puoi compilare tu i campi, ma
fermati sempre prima di salvare o pubblicare.

STEP 9. Test finale
Crea lavoro/09-test.md e guidami a testare ogni funnel come se fossi una
cliente: commento → DM → iscrizione → email (controlla anche lo spam) → guida
scaricabile → acquisto di prova → email di consegna → stop follow-up. Per ogni
punto che non funziona, dammi le 2-3 cause più probabili e la soluzione.

Inizia ora dallo STEP 1.
```
