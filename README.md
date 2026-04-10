# Codice sconto Sephora, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Sephora** da [shopilo.it](https://shopilo.it/negozi/sephora.it). Restituisce **coupon Sephora** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-sephora](https://shopilo-it.github.io/codice-sconto-sephora/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-sephora
cd codice-sconto-sephora
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Sephora",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su make-up e skincare premium",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/sephora.it"
  }
]
```

## Coupon Sephora disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su make-up e skincare premium | [shopilo.it](https://shopilo.it/negozi/sephora.it) |

Codici attivi: **[shopilo.it/negozi/sephora.it](https://shopilo.it/negozi/sephora.it)**

## Domande frequenti

### Come utilizzo un codice sconto Sephora?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/sephora.it), aggiungi i prodotti al carrello su Sephora e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Sephora?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Sephora piu recenti?
La pagina [shopilo.it/negozi/sephora.it](https://shopilo.it/negozi/sephora.it) viene aggiornata quotidianamente con i codici sconto Sephora, voucher Sephora e coupon promozionali Sephora piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Sephora

Sephora e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/sephora.it) trovi i migliori codici sconto Sephora, coupon Sephora verificati e voucher Sephora attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-sephora
```

```javascript
const { fetchCoupons } = require('codice-sconto-sephora');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
