# Prototype — 15 questions + export Excel (Flask)

## Local (PC)
Dans PyCharm > Terminal:
    python -m pip install -r requirements.txt
    python app.py
Puis ouvre:
    http://127.0.0.1:8000

## Partager à un pote via un vrai lien (sans installer Python chez lui)
➡️ Déploiement gratuit (prototype) sur Render

1) Mets ce dossier sur GitHub (un repo)
2) Render.com -> New -> Web Service -> connecte le repo
3) Settings Render:
   - Build command:
       pip install -r requirements.txt
   - Start command:
       gunicorn app:app
4) Render te donne une URL du type:
       https://xxxx.onrender.com
Ton pote clique, ça marche.

Note: les services gratuits Render peuvent "sleep" après ~15 min sans trafic et mettre ~1 min à redémarrer.

## Où est l’Excel ?
- En local: dossier ./data
- Sur un hébergeur gratuit: l’espace disque peut être temporaire.
  Pour une vraie collecte, il faudra plutôt envoyer les résultats vers une base de données ou Google Sheets.
