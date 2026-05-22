# Upload Matrix Symbalyx

Le dossier Matrix à pousser vient du ZIP local `symbalyx-ia-main.zip`.

Chemin à extraire depuis le ZIP :

```txt
symbalyx-ia-main/matrix/
```

Contenu Matrix attendu :

```txt
matrix/.gitignore
matrix/COMPARATIF.md
matrix/GUIDE.md
matrix/README.md
matrix/SECURITY.md
matrix/docker-compose.yml
matrix/bots/Dockerfile
matrix/bots/assistant.py
matrix/bots/requirements.txt
matrix/config/Caddyfile
matrix/config/livekit.yaml
matrix/config/nginx-ui.conf
matrix/config/synapse-overrides-v2.yaml
matrix/config/turnserver.conf
matrix/element/config.json
matrix/element-call/config.json
matrix/ui/icon.svg
matrix/ui/index.html
matrix/ui/manifest.json
matrix/ui/service-worker.js
matrix/ui/templates.js
```

Commande locale recommandée depuis Windows PowerShell :

```powershell
cd $env:USERPROFILE

git clone https://github.com/arsenevaslin12-png/LLM-private.git
cd LLM-private

# Copier ici le dossier matrix extrait du ZIP, puis :
git add matrix
git commit -m "Add Matrix Symbalyx stack"
git push origin main
```

⚠️ À vérifier avant publication : ce repo est actuellement public. Les fichiers Matrix contiennent des secrets par défaut de développement comme `synapse_local_pw_change_me`, `symbalyx_turn_secret_change_me` et `symbalyx_lk_secret_change_me_min_32_chars`. Ces valeurs doivent être changées avant un vrai déploiement.