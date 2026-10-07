# Vibe — installeurs

Ce dépôt ne contient pas de code : il **distribue les installeurs de Vibe**
pour Linux, Windows et macOS. Le code source est privé.

Vibe est un lecteur de musique local, rapide et sobre. Il lit votre musique là
où elle se trouve — rien n'est copié, rien n'est modifié — l'affiche
proprement et la joue sans blanc entre les morceaux, touches média de l'OS
comprises. Moteur audio en Rust (MP3, FLAC, OGG, M4A/AAC, ALAC, WAV, AIFF),
paroles synchronisées, reconnaissance d'un morceau au son, et un accent
d'interface qui suit la pochette en cours.

## Télécharger

**[→ Dernière version](https://github.com/Corneille9/vibe-releases/releases/latest)**
· ou depuis [corneille.vercel.app/telechargements](https://corneille.vercel.app/telechargements)

| Système | Fichier |
| --- | --- |
| Debian, Ubuntu | `Vibe_<version>_amd64.deb` |
| Fedora, RHEL | `Vibe-<version>-1.x86_64.rpm` |
| Toute distribution Linux | `Vibe_<version>_amd64.AppImage` |
| Windows 10 / 11 | `Vibe_<version>_x64-setup.exe` |
| macOS 11+ (Intel et Apple Silicon) | `Vibe_<version>_universal.dmg` |

## Installer

```sh
# Debian / Ubuntu
sudo dpkg -i Vibe_*_amd64.deb

# Fedora
sudo dnf install Vibe-*.x86_64.rpm

# AppImage : rien à installer, juste à rendre exécutable
chmod +x Vibe_*.AppImage && ./Vibe_*.AppImage
```

Sur **Windows**, l'installeur n'est pas signé : SmartScreen affiche un
avertissement, choisissez « Informations complémentaires » puis « Exécuter
quand même ». Sur **macOS**, le binaire n'est pas signé non plus : au premier
lancement, clic droit sur l'application puis « Ouvrir ».

Les données de l'application vivent dans le dossier de l'OS
(`~/.local/share/app.vibe.player` sous Linux) : `vibe.db` et `covers/`.

## Publication

Les fichiers sont construits et attachés ici automatiquement par le workflow
`release.yml` du dépôt source, à chaque tag `v*`. Ce dépôt n'est jamais
modifié à la main.

---

Par **Corneille BANKOLE** — [corneille.vercel.app](https://corneille.vercel.app/)
· [GitHub](https://github.com/Corneille9)
