#CORRESPONDANCES BASH SHELL ET POWERSHELL

| COMMANDE BASH SHELL  | ACTION  | COMMANDE POWERSHELL  |
|---|---|---|
| __cp__ fichier.md ~/Téléchargements/fichier.md  | Copie le fichier fichier.md du répertoire où nous sommes vers le dossier Téléchargements, on aurait pu changer le nom de la copie en changeant le nom du fichier de destination  | __Copy-Item__ -Path "./fichier.md" -Destination "~/Téléchargements/fichier.md"  |
| __rm__ fichier.file| supprime le fichier ou dossier en ajoutant -r (dans bash)  | __Remove-Item__ -Path "./fichier.file"  |
| __cd__ Téléchargements | se déplacer, changer de répertoire (de dossier), ici, nous sommes dans homme/user et nous voulons rentrer dans Téléchargements  |  __Set-Location -Path__ "~/Téléchargements |
| __mkdir__ NouveauDossier | Créer un dossier dans le dossier où nous sommes  | __New-Item__ -ItemType Directory -Path ./NouveauDossier  |
| __man__ mkdir | ouvre une aide sur l'utilisation de la commande (ici mkdir en bash, New-Item en Powershell)  | __get-help__ new-item  |
| __history__  | Affiche l'historique des dernières commandes saisies  | __history__  |
| __alias__ c="clear" | créé un raccourci, ici la commande clear pourra ensuite se taper c   | __New-Alias__ -Name "c" clear  |
| __cat__ file.txt | Affiche le contenu d'un fichier, ici file.txt  | __get-content__ file.txt  |
