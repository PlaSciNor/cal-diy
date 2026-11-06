# cal-diy (Planète Sciences Normandie)

Compilation de l'image Docker de [Cal.diy](https://github.com/calcom/cal.diy) (version libre MIT de Cal.com)
pour la prise de rendez-vous en ligne sur https://rdv.plasci-normandie.org.

- La compilation se fait sur les machines GitHub Actions (le serveur n'est pas assez puissant).
- Image publiée : `ghcr.io/plascinor/cal-diy:<commit>` et `:latest`.
- Mettre à jour : changer le commit dans `CAL_DIY_REF` (ou lancer le workflow à la main avec un autre `ref`),
  puis sur le serveur : `cd /opt/docker/rdv && docker compose pull && docker compose up -d`.
- Aucun secret ni donnée dans ce dépôt : la configuration réelle (`.env`) reste sur le serveur.
