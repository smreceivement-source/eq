# Prompt: pagine di vendita per Systeme

Questo prompt crea le pagine **già impaginate**, pronte da incollare in Systeme.

**Come funziona:**
- Claude Code scrive il codice delle pagine e un'**anteprima** da aprire in Chrome. La guardiamo insieme e la correggiamo finché va bene.
- In Systeme la pagina diventa **un blocco "HTML/codice personalizzato" con il testo e la grafica**, più il **modulo nativo di Systeme** (iscrizione o pagamento). Il modulo deve restare quello di Systeme, altrimenti non partono le automazioni e i pagamenti.
- Il codice lo incolli tu, oppure lo fa Claude in Chrome direttamente nell'editor di Systeme.

Usalo dopo lo STEP 2 del prompt di avvio, quando esiste già il file `CLAUDE.md` con il brief.

```
Crea le pagine di vendita dei miei due funnel per Systeme.io. Usa CLAUDE.md per
brief, tono e prezzi, i PDF in guide/ per i contenuti e i file in materiali/ per
logo, foto, copertine, recensioni e colori. Usa solo recensioni presenti in
materiali/: se non ce ne sono, togli la sezione. Non inventarle mai.

COSA DEVI PRODURRE (nella cartella pagine/)
Per ciascun funnel (A e B), 2 pagine:
1. ISCRIZIONE (guida gratis): sopra-titolo, titolo, sottotitolo, mockup della
   guida, 3-4 punti "cosa trovi dentro", [QUI MODULO SYSTEME: nome + email],
   nota privacy, mini "chi sono".
2. OFFERTA (si apre subito dopo l'iscrizione): è la pagina più importante.
   Struttura in quest'ordine:
   a. barra di conferma: "✅ La tua guida gratuita sta arrivando via email" +
      barra di avanzamento "Passo 2 di 2"
   b. hero: titolo con la promessa della guida a pagamento, sottotitolo,
      mockup, bottone che scorre al modulo d'ordine
   c. "Ti riconosci?": 3-4 situazioni concrete del mio pubblico
   d. la soluzione: presentazione della guida e perché è il passo naturale dopo
      quella gratuita
   e. cosa trovi dentro: 6 punti con icona, presi dal PDF vero
   f. per chi è / per chi non è (2 colonne)
   g. chi sono: foto + 3 righe
   h. recensioni (solo se esistono)
   i. box dell'offerta: cosa ricevi, prezzo pieno barrato SOLO se esiste
      davvero, prezzo lancio, scadenza solo se reale
   j. [QUI MODULO D'ORDINE SYSTEME CON ORDER BUMP]
   k. garanzia (solo se l'ho decisa nel brief)
   l. 5 domande frequenti a fisarmonica (formato, come la ricevo, quanto tempo
      serve, per chi è, pagamento sicuro)
   m. bottone finale + link piccolo "No grazie, voglio solo la guida gratuita"
   n. piè di pagina: dati legali, link privacy e condizioni

DESIGN (deve sembrare il mio profilo Instagram: settore immobiliare/interior,
minimal ma valorizzante e di stile)
- Palette calda e neutra: fondo avorio/sabbia (#F5F0E8 circa), testo
  marrone-taupe scuro (#3B302A circa), linee sottili color tortora. Accento per
  bottoni e dettagli: bordeaux (#7A1F2B circa). Colori secondari da usare con
  moderazione: blu polvere (#8FA3B8), cioccolato (#5A3A2A), verde salvia (#8A9A86).
  Se in materiali/ c'è colori.txt, quello ha la precedenza.
- Tipografia come nei miei post: titoli in serif elegante e sottile (es.
  Cormorant Garamond) con UNA parola chiave in corsivo per titolo (es. "Quest'anno
  il *Natale* lo crei tu"); firma "SIRIANA FINOTTI" in maiuscoletto piccolo con
  lettere molto spaziate, sopra una linea sottile corta; testo in sans-serif
  pulito (es. Jost o Montserrat light/regular).
- Tanto spazio vuoto, foto di interni grandi e luminose, angoli appena
  arrotondati o netti, niente ombre pesanti, niente emoji nei titoli, niente
  colori accesi o effetti "da marketing aggressivo". Bottoni sobri: pieni in
  bordeaux con testo avorio, oppure bordo sottile.
- Le immagini sono la parte più importante: usa le foto di interni e le
  copertine in materiali/, a tutta larghezza nell'hero.
- Mobile first: la maggior parte arriva da Instagram, quindi deve essere perfetta
  sul telefono (testo minimo 17px, bottoni grandi, una colonna).
- Bottoni con testi d'azione specifici, mai solo "Acquista".
- Il funnel A ha un tocco natalizio discreto (solo nella pagina gratis); il
  funnel B ha uno stile più "business ospitalità".

REGOLE TECNICHE (importanti per Systeme)
- Per ogni pagina, dividi il codice in BLOCCHI separati da incollare in blocchi
  "HTML/codice personalizzato" di Systeme: un blocco PRIMA del modulo Systeme e
  uno DOPO. Salvali come pagine/A-offerta-blocco-1.html, ...-blocco-2.html ecc.
- Ogni blocco deve funzionare da solo: CSS dentro un tag <style> nel blocco,
  tutte le classi con il prefisso "gp-" per non rompere lo stile di Systeme,
  niente librerie esterne tranne Google Fonts, JavaScript solo se indispensabile
  (fisarmonica FAQ e scorrimento al modulo).
- Il bottone "scorri al modulo" deve puntare all'ancora #ordine: dimmi come dare
  questo ID alla sezione del modulo in Systeme.
- Le immagini: usa per ora i file in materiali/ per l'anteprima, poi dimmi
  quali caricare nella libreria media di Systeme e dove sostituire gli indirizzi
  delle immagini.

ANTEPRIMA
Crea pagine/anteprima-A-offerta.html (e le altre) che uniscono i blocchi e al
posto del modulo Systeme mostrano un riquadro grigio "MODULO SYSTEME". Aprile in
Chrome, prima in versione desktop e poi simulando il telefono, e chiedimi cosa
cambiare. Correggi finché non scrivo "approvata".

DOPO L'APPROVAZIONE
Scrivi pagine/ISTRUZIONI-SYSTEME.md con i passaggi esatti: quale modello di
pagina vuota scegliere, dove aggiungere i blocchi HTML, dove inserire il modulo
nativo, come attivare l'order bump, come impostare l'ID #ordine, come
collegare la pagina di iscrizione alla pagina offerta e come controllare
l'anteprima mobile di Systeme.
Se ho attiva l'estensione Claude in Chrome, chiedimi se vuoi che lo faccia tu
nell'editor di Systeme. In quel caso lavora una pagina alla volta e fermati
SEMPRE prima di salvare o pubblicare.

Inizia dal funnel A, pagina OFFERTA.
```
