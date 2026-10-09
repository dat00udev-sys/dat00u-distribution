# Installer Zaphir

## Avant de commencer

Il vous faut :
- un appareil sous Android 8 ou version suivante : Android TV, Google TV, Fire TV, box, téléphone ou tablette ;
- une connexion Internet ;
- votre propre source IPTV.

Aucun compte Zaphir ni compte GitHub n'est nécessaire.

Le fichier à installer est **Zaphir-0.11.2.apk**, dans les *Assets* de la [Release 0.11.2](https://github.com/dat00udev-sys/dat00u-distribution/releases/tag/v0.11.2). Les archives « Source code » ne sont pas l'application.

## Sur un téléphone ou une tablette

1. Ouvrez la Release dans le navigateur et téléchargez **Zaphir-0.11.2.apk**.
2. Ouvrez le fichier téléchargé. Si Android le demande, autorisez l'installation depuis ce navigateur ; le nom du réglage varie selon l'appareil.
3. Confirmez l'installation, puis ouvrez **Zaphir** et ajoutez votre source.

## Sur une TV, une Fire TV ou une box

Les TV n'ont en général pas de navigateur. Choisissez l'une de ces méthodes :

- **Avec l'application Downloader** (disponible dans les boutiques Google TV et Amazon) :
  1. tapez l'adresse du fichier :
     `https://github.com/dat00udev-sys/dat00u-distribution/releases/download/v0.11.2/Zaphir-0.11.2.apk`
  2. autorisez Downloader à installer des applications quand la TV le demande ;
  3. confirmez l'installation.
- **Depuis un ordinateur, avec le débogage activé sur la TV :**
  ```
  adb connect <adresse IP de la TV>
  adb install Zaphir-0.11.2.apk
  ```

## Mettre à jour sans perdre vos données

Zaphir vérifie lui-même s'il existe une nouvelle version et affiche un bandeau sur l'accueil. Appuyez sur **« Mettre à jour »** :
- **Sur téléphone :** le fichier s'ouvre dans le navigateur.
- **Sur TV :** l'application télécharge elle-même la nouvelle version et ouvre l'installateur d'Android. La première fois, la TV vous demande d'autoriser Zaphir à installer des applications.

Installez toujours **par-dessus** la version existante, sans désinstaller : vos sources, favoris et réglages sont conservés, car les mises à jour officielles ont la même signature.

L'application « Zaphir (dev) » est réservée aux tests. Elle est distincte et n'est pas distribuée.

## Vérifier le fichier

Le fichier `SHA256SUMS.txt` contient l'empreinte de chaque APK. Pour la contrôler sous PowerShell :

```powershell
Get-FileHash .\Zaphir-0.11.2.apk -Algorithm SHA256
```
