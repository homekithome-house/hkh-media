# PÉRIMÈTRE — HKH/Media
nature: produit · departement: marketing

## Mission (1 phrase)
Servir de dépôt distant public des visuels HKH publiés — URL publique stable exigée par l'API Meta et les autres plateformes, hors du repo de code.

## Je possède (source de vérité — fait foi en cas de doublon)
- Visuels publiés bruts : `posts/{YYYY-MM}/{NNN}-{slug}/image-1.jpg` (copie de publication, jamais la référence — cf. Interfaces).

## Je fais / je ne fais PAS
- ✅ Héberger les JPEG que `HKH/Marketing/outils/media-publier.sh` copie ici, servis publiquement en URL raw GitHub.
- ⛔ Je ne suis PAS la source de vérité du visuel (le rendu original, son verdict, ses métadonnées) → `HKH/Visual-Pipeline/renders/_valides/` + `registres/tirages.csv`.
- ⛔ Je ne décide rien (pas de validation, pas de choix éditorial) — pur stockage dérivé.
- ⛔ Jamais un visuel non validé, jamais un fichier de prix, de prospect, ou un secret — ce dépôt est **public**.

## Interfaces
- **J'entre** : rien (pas de pull actif — je reçois en écriture depuis `HKH/Marketing/outils/media-publier.sh`).
- **Je sors** : les fichiers médias servis en URL raw GitHub (`HKH_MEDIA_BASE_URL`), consommés par le job de publication (A3b) et les plateformes tierces.
- **Miroirs** : `HKH/Visual-Pipeline/renders/_valides/` **fait foi** (le rendu source et son verdict) ; ce repo est le miroir publié, rafraîchi par copie depuis `HKH/Marketing/outils/media-publier.sh`.

## M'adresser un travail
cwd=`/Users/benjamindupouy/Developer/Claude-Projet/HKH/Media` — usage attendu quasi nul en écriture directe : les écritures normales passent par `HKH/Marketing/outils/media-publier.sh`, pas par une session ouverte ici.
