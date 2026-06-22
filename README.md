# Dépôt alkoFlix 1.0

Dépôt Kodi officiel pour alkoFlix et ses extensions associées.

## Versions incluses

- Dépôt Kodi : `repository.alkoflix` version `1.0`
- Extension vidéo : `plugin.video.alkoflix` version `2.0`

## Installation

1. Dans Kodi, aller dans `Paramètres > Gestionnaire de fichiers`.
2. Choisir `Ajouter une source`.
3. Ajouter l’URL : `https://lesalkodiques.github.io/`.
4. Donner un nom à la source, par exemple : `Les alKODIques`.
5. Aller dans `Extensions > Installer depuis un fichier ZIP`.
6. Ouvrir la source `Les alKODIques`.
7. Installer `repository.alkoflix-1.0.zip`.
8. Aller dans `Extensions > Installer depuis un dépôt > Dépôt alkoFlix`.
9. Installer `alkoFlix`.

Une fois le dépôt installé, les prochaines mises à jour d’alkoFlix seront proposées automatiquement par Kodi.

## Structure GitHub attendue

À la racine du dépôt GitHub `repository.alkoflix`, il doit y avoir :

```text
LICENSE
README.md
addons.xml
addons.xml.md5
plugin.video.alkoflix/
repository.alkoflix/
repository.alkoflix-1.0.zip
```

## Règle pour les prochaines mises à jour

Pour publier une future version d’alkoFlix :

1. Ajouter le nouveau zip dans `plugin.video.alkoflix/`, par exemple `plugin.video.alkoflix-2.0.1.zip`.
2. Modifier la version de `plugin.video.alkoflix` dans `addons.xml`.
3. Regénérer `addons.xml.md5` à partir du nouveau `addons.xml`.
4. Commit les trois éléments ensemble.

Ne pas modifier `addons.xml` directement sans regénérer `addons.xml.md5`.
