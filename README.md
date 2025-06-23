# Documentation de l'expérimentation sur les images satellites

## Contenu du site

Le site contient :

- De la documentation sur toutes les parties de l'expérimentation ;
- Un document de travail résumant une partie des travaux conduits au cours de l'expérimentation ;
- Les slides présentées lors du séminaire de fin d'expérimentation le 28/05/24 à la Dirag ;
- L'enregistrement vidéo du séminaire ;
- Le lien vers l'application de visualisation ;
- Une présentation réalisée pour le workshop AIML4OS Earth Observation ;  
- Le séminaire DMCSI sur le sujet des données satellites : Utilisation des images satellites pour améliorer le repérage des logements dans les départements d'outre-mer.  

## Build

Pour build le site de documentation, il faut installer une pre-release de Quarto:

```sh
wget https://github.com/quarto-dev/quarto-cli/releases/download/v1.5.37/quarto-1.5.37-linux-amd64.deb -O quarto.deb
sudo dpkg -i quarto.deb
quarto check install
rm quarto.deb
```

Pour render le site, exécutez la commande suivante depuis la racine du projet

```sh
quarto preview --host 0.0.0.0 --port 5000
```

Fermer le site ouvert sur le port 5000 :

```sh
fuser -k 5000/tcp
```