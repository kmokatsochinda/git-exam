# git-exam

Petit projet Go minimal qui démarre un serveur HTTP sur le port 8080.

## Prérequis

- Go 1.20+ installé sur la machine

## Exécution

Depuis la racine du projet :

```powershell
# lancer directement
go run .

# ou compiler puis exécuter
go build .
.\git-exam.exe
```

## Test rapide

Une fois le serveur démarré, tester avec PowerShell :

```powershell
Invoke-WebRequest -Uri http://localhost:8080 -UseBasicParsing
# ou
curl http://localhost:8080
```

Le serveur n'enregistre actuellement aucun handler HTTP personnalisé, donc il renverra 404 par défaut.

## Gitignore

Le fichier `.gitignore` du dépôt contient au moins :

- `go.mod`
- `.DS_Store`

Si tu veux que le `.gitignore` soit restreint uniquement à ces deux lignes, dis‑le et je le modifie.

## Modifications proposées (optionnel)

- Ajouter un handler racine `/` pour répondre `ok` afin de tester plus facilement.
- Ajouter des tests unitaires pour le handler.

## Auteur

Ce dépôt appartient à `kmokatsochinda`.


