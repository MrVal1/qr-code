# QR Studio Ultimate

Générateur de QR codes 100% personnalisable (formes, dégradés, fond transparent PNG, SVG, logo central, Wi-Fi, vCard, etc.), prêt à être déployé sur **Portainer**.

## Déploiement sur Portainer (via Git)

1. Dans Portainer : **Stacks** → **Add stack** → **Repository**.
2. Renseignez :
   - **Repository URL** : `https://github.com/MrVal1/qr-code`
   - **Repository reference** : `refs/heads/main`
   - **Compose path** : `docker-compose.yml`
3. *(Optionnel)* Si le port par défaut **`47831`** est déjà pris, ajoutez une variable d'environnement `PORT` dans Portainer (ex. `PORT=52914`).
4. Cliquez sur **Deploy the stack**.

L'application sera accessible sur `http://<IP-DE-VOTRE-SERVEUR>:47831`.

## Déploiement en ligne de commande

```bash
docker compose up -d --build
```
