# Minuit 64

Boutique de voitures miniatures au 1:64, garages LED et guides de collection.

L’archive contient les fichiers du site, les scripts de génération et le code du paiement de test.

## Publication sur Render

Type de service « Static Site », offre gratuite.

Commande de génération

```sh
unzip -oq minuit64-source.zip && node minuit64/scripts/render.mjs public "$RENDER_EXTERNAL_URL"
```

Dossier de publication `public`.

La route `/api/*` doit être réécrite vers `https://minuit64.pages.dev/api/*`.
Le service de paiement Cloudflare doit autoriser l’origine Render dans `PUBLIC_SHOP_ORIGIN`.
La clé Stripe est stockée dans Cloudflare.
