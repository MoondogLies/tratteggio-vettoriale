# tratteggio-vettoriale
Convertitore immagine → tratteggio vettoriale SVG

## Rimuovi sfondo

La modalità «Rimuovi sfondo» scontorna il soggetto ed esporta un SVG trasparente
(foto ritagliata, tracciato vettoriale a colori o sagoma).

- **IA**: usa il modello [RMBG-1.4](https://huggingface.co/briaai/RMBG-1.4) di BRIA AI
  tramite [transformers.js](https://github.com/huggingface/transformers.js), eseguito
  interamente nel browser (l’immagine non viene inviata a nessun server). Al primo uso
  scarica circa 44 MB da jsDelivr e Hugging Face. **Il modello è gratuito solo per uso
  non commerciale**: per usi commerciali serve una licenza BRIA.
- **Sfondo a tinta unita**: metodo senza IA, offline, adatto a loghi e foto di prodotto.
