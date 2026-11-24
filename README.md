# tratteggio-vettoriale
Convertitore immagine → tratteggio vettoriale SVG

## Rimuovi sfondo

La modalità «Rimuovi sfondo» scontorna il soggetto ed esporta un SVG trasparente:
come foto ritagliata oppure, con la spunta «Converti in tracciati SVG», come path
vettoriali (numero di colori automatico o scelto, oppure sagoma in un colore).
Il metodo «Automatico» usa il metodo senza IA quando il fondo è uniforme (tipico
dei loghi) e l’IA negli altri casi.

- **IA**: usa il modello [RMBG-1.4](https://huggingface.co/briaai/RMBG-1.4) di BRIA AI
  tramite [transformers.js](https://github.com/huggingface/transformers.js), eseguito
  interamente nel browser (l’immagine non viene inviata a nessun server). Al primo uso
  scarica circa 44 MB da jsDelivr e Hugging Face. **Il modello è gratuito solo per uso
  non commerciale**: per usi commerciali serve una licenza BRIA.
- **Sfondo a tinta unita**: metodo senza IA, offline, adatto a loghi e foto di prodotto.
