# Cod reducere Nailsup — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Nailsup** de pe [shopilo.ro](https://shopilo.ro/magazin/nailsup.ro). Returneaza **cupoane Nailsup** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-nailsup](https://shopilo-ro.github.io/cod-reducere-nailsup/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-nailsup
cd cod-reducere-nailsup
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Nailsup",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la produse nail art",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/nailsup.ro"
  }
]
```

## Cupoane Nailsup disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la produse nail art | [shopilo.ro](https://shopilo.ro/magazin/nailsup.ro) |

Codurile active: **[shopilo.ro/magazin/nailsup.ro](https://shopilo.ro/magazin/nailsup.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Nailsup?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/nailsup.ro), adauga produsele in cos pe Nailsup, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Nailsup?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Nailsup?
Pagina [shopilo.ro/magazin/nailsup.ro](https://shopilo.ro/magazin/nailsup.ro) este actualizata zilnic cu cele mai noi cod reducere Nailsup, voucher Nailsup si cupon promotional Nailsup.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Nailsup

Nailsup este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/nailsup.ro) cele mai bune cod reducere Nailsup, cupoane Nailsup verificate si voucher Nailsup active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-nailsup
```

```javascript
const { fetchCoupons } = require('cod-reducere-nailsup');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
