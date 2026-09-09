# GENUC Mobile — livraisons

Ce dépôt sert **uniquement à distribuer l'application mobile GENUC** à l'équipe.
Il ne contient aucun code source : le projet vit dans un dépôt privé, et seuls
les fichiers d'installation sont publiés ici.

## Télécharger la dernière version

👉 **[Aller à la dernière version](https://github.com/bamochris/genuc-mobile-releases/releases/latest)**

Sur la page qui s'ouvre, ouvrez la section **Assets** et touchez le fichier
`.apk`. Aucun compte GitHub n'est nécessaire.

## Installer sur Android

1. Ouvrir le fichier `.apk` téléchargé (dans « Téléchargements »).
2. Android demandera d'autoriser l'installation depuis cette source : accepter.
3. L'installation par-dessus une version précédente conserve les données — il
   n'est pas nécessaire de désinstaller l'ancienne.

Toutes les versions publiées ici sont signées avec la même clé
(`CN=GENUC Mobile`). Si Android refuse l'installation en parlant de signature,
c'est que l'application installée ne vient pas d'ici : la désinstaller d'abord.

## Vérifier que le fichier est intact

Chaque version indique l'empreinte **SHA-1** du fichier dans ses notes. Pour la
contrôler avant installation :

```powershell
Get-FileHash .\genuc-mobile-AAAA-MM-JJ.apk -Algorithm SHA1
```

## Signaler un problème

Précisez la **date de la version** installée (elle figure dans le nom du
fichier), l'écran concerné et ce que vous attendiez. Les journaux du serveur ne
disent rien d'un écran qui affiche une valeur fausse — c'est votre description
qui permet de le retrouver.
