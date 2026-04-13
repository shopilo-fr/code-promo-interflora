# Code promo Interflora, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Interflora** depuis [shopilo.fr](https://shopilo.fr/reductions/interflora.fr). Renvoie les **coupons Interflora** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-interflora](https://shopilo-fr.github.io/code-promo-interflora/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-interflora
cd code-promo-interflora
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Interflora",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur la livraison de bouquets",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/interflora.fr"
  }
]
```

## Coupons Interflora disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur la livraison de bouquets | [shopilo.fr](https://shopilo.fr/reductions/interflora.fr) |

Codes actifs : **[shopilo.fr/reductions/interflora.fr](https://shopilo.fr/reductions/interflora.fr)**

## Questions frequentes

### Comment utiliser un code promo Interflora ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/interflora.fr), ajoutez les produits a votre panier sur Interflora et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Interflora ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Interflora les plus recents ?
La page [shopilo.fr/reductions/interflora.fr](https://shopilo.fr/reductions/interflora.fr) est mise a jour quotidiennement avec les codes promo Interflora, bons de reduction Interflora et coupons promotionnels Interflora les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Interflora

Interflora est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/interflora.fr), retrouvez les meilleurs codes promo Interflora, coupons Interflora verifies et bons de reduction Interflora actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-interflora
```

```javascript
const { fetchCoupons } = require('code-promo-interflora');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
