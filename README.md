# Codice sconto GioiaPura, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto GioiaPura** da [shopilo.it](https://shopilo.it/negozi/gioiapura.it). Restituisce **coupon GioiaPura** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-gioiapura](https://shopilo-it.github.io/codice-sconto-gioiapura/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-gioiapura
cd codice-sconto-gioiapura
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "GioiaPura",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su gioielli e orologi",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/gioiapura.it"
  }
]
```

## Coupon GioiaPura disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su gioielli e orologi | [shopilo.it](https://shopilo.it/negozi/gioiapura.it) |

Codici attivi: **[shopilo.it/negozi/gioiapura.it](https://shopilo.it/negozi/gioiapura.it)**

## Domande frequenti

### Come utilizzo un codice sconto GioiaPura?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/gioiapura.it), aggiungi i prodotti al carrello su GioiaPura e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon GioiaPura?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher GioiaPura piu recenti?
La pagina [shopilo.it/negozi/gioiapura.it](https://shopilo.it/negozi/gioiapura.it) viene aggiornata quotidianamente con i codici sconto GioiaPura, voucher GioiaPura e coupon promozionali GioiaPura piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su GioiaPura

GioiaPura e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/gioiapura.it) trovi i migliori codici sconto GioiaPura, coupon GioiaPura verificati e voucher GioiaPura attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-gioiapura
```

```javascript
const { fetchCoupons } = require('codice-sconto-gioiapura');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
