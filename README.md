# git-exam

Petit projet Go minimal qui démarre un serveur HTTP sur le port 8080.

## Exécution

Depuis la racine du projet :

```powershell
# lancer directement
go run .

# ou compiler puis exécuter
go build .
.\git-exam.exe
```

## Notes

- Le fichier `.gitignore` contient des règles pour ignorer `go.mod` et `.DS_Store`.
- Le serveur actuel n'enregistre aucun handler, donc les requêtes retournent 404 par défaut.
