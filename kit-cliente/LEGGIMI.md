# Kit funnel guide: istruzioni

Bastano 3 passi.

1. **Metti i PDF nelle cartelle giuste**, dentro `guide/`:
   - `1-natale-GRATIS`: la guida gratuita di Natale
   - `2-valorizzazione-casa-PAGAMENTO`: la guida a pagamento sulla valorizzazione della casa
   - `3-percezione-affitto-GRATIS`: la guida gratuita per migliorare la percezione della casa in affitto
   - `4-case-che-vendono-PAGAMENTO`: la guida a pagamento "Case che vendono"

2. **Apri Claude Code dentro questa cartella** (`kit-cliente`).

3. **Copia tutto il testo del riquadro in `PROMPT-AVVIO.md` e incollalo** in Claude Code.
   Claude lavora uno step alla volta e si ferma sempre ad aspettare il tuo "ok".
   Tutto quello che prepara viene salvato nella cartella `lavoro/`.

Se interrompi il lavoro, quando riapri Claude Code in questa cartella scrivi:
`Riprendi dallo step a cui eravamo arrivati (guarda lavoro/stato.md).`
