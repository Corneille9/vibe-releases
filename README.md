# Vibe

Lecteur de musique local, rapide et sobre, disponible sur Linux, Windows et
macOS.

Vibe lit votre bibliothèque directement dans vos dossiers, sans jamais copier ni
modifier un fichier. Le scan est récursif et incrémental, les pochettes, les
albums et les compilations sont reconnus, et la lecture s'enchaîne sans blanc
entre les morceaux.

Le moteur audio est écrit en Rust et traite les mêmes formats sur les trois
systèmes : MP3, FLAC, OGG, M4A/AAC, ALAC, WAV et AIFF. S'y ajoutent les paroles
synchronisées, la correction des métadonnées, la reconnaissance d'un morceau au
son et l'intégration aux touches média du système.

## Télécharger

[**→ Dernière version**](https://github.com/Corneille9/vibe-releases/releases/latest)
· ou depuis [corneille.vercel.app/telechargements](https://corneille.vercel.app/telechargements)

| Système | Fichier |
| --- | --- |
| Debian, Ubuntu | `Vibe_<version>_amd64.deb` |
| Fedora, RHEL | `Vibe-<version>-1.x86_64.rpm` |
| Autres distributions Linux | `Vibe_<version>_amd64.AppImage` |
| Windows 10 et 11 | `Vibe_<version>_x64-setup.exe` |
| macOS 11 et plus (Intel et Apple Silicon) | `Vibe_<version>_universal.dmg` |

## Installer

**Debian, Ubuntu**

```sh
sudo dpkg -i Vibe_*_amd64.deb
```

**Fedora, RHEL**

```sh
sudo dnf install Vibe-*.x86_64.rpm
```

**Autres distributions Linux**

```sh
chmod +x Vibe_*.AppImage
./Vibe_*.AppImage
```

**Windows** : lancez l'installeur. Si un avertissement SmartScreen s'affiche,
choisissez « Informations complémentaires » puis « Exécuter quand même ».

**macOS** : ouvrez le `.dmg` et glissez Vibe dans Applications. Au premier
lancement, faites un clic droit sur l'application puis « Ouvrir ».

## Configuration requise

- Linux : WebKitGTK 4.1 et ALSA (Ubuntu 22.04+, Fedora 38+)
- Windows 10 ou 11, 64 bits
- macOS 11 Big Sur ou plus récent, Intel ou Apple Silicon

---

Par **Corneille BANKOLE** · [corneille.vercel.app](https://corneille.vercel.app/)
· [GitHub](https://github.com/Corneille9)
