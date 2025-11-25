# SAOBOT – Valorant Colorbot Suite

![Saobot logo](saobot.ico)

**Saobot** est une interface premium qui réunit colorbot, overlay FOV évolué et module de spoofing USB autour d’une expérience inspirée de Valorant. L’objectif est de montrer comment automatiser la vision par couleur, l’intégration Arduino et le pilotage d’outils temps réel dans un cadre éducatif. Toute diffusion vise la recherche et l’apprentissage : l’utilisateur final est seul responsable de l’usage qu’il en fait.

> ⚠️ **Avertissement pédagogique** – Saobot est fourni pour illustrer des concepts (vision couleur, hooking d’événements, automatisation HID). Nous ne cautionnons ni n’encourageons une utilisation contraire aux CGU de Riot Games ou d’un tiers. En téléchargeant ce dépôt vous acceptez d’assumer l’entière responsabilité des actions menées avec le logiciel.

---

## Pourquoi Saobot ?

- **Expérience unifiée** : login premium, dashboard modulaire, télémétrie live et sauvegarde auto des profils.
- **Contrôle chirurgical** : overlay FOV ultra-fin (circle/square/triangle/star/heart), clignotement RGB, stroke dynamique et transparence totale.
- **Automations combo** : aimbot, triggerbot et anti-recul fonctionnent ensemble ou séparément avec profils tête/corps/pieds, offsets précis et temps de réaction au milliseconde.
- **Spoofing intégré** : flash Arduino Leonardo, clonage VID/PID et scripts CLI sans quitter l’app, idéal pour étudier la chaîne complète capture ➜ HID.
- **Observabilité** : panneau systèmes, FPS capture, statut Arduino, logs temps réel, crash reporter dédié.
- **Stack moderne** : PyQt5, numpy, dxcam/d3dshot, pyserial, packaging PyInstaller (Saobot.exe) prêt à diffuser.

## Fonctionnalités détaillées

- **Portail de licence** : panneau « ACCÈS PREMIUM » avec ouverture de ticket/support rapide (Discord & site `https://saobot.shop`).
- **Command Center** :
  - *General* – backends de capture (dxcam/d3dshot), throttling, preview basse latence.
  - *FOV Overlay* – formes multiples, animations RGB, blink, stroke ajustable.
  - *Aimbot* – vitesses X/Y indépendantes, offsets dynamiques, profils présets, safe-mode pour humains.
  - *Triggerbot* – délais personnalisables, filtres de couleur, zones flexibles.
  - *Anti-Recoil* – courbes personnalisées par arme/profil.
  - *Spoofing* – détection HID, clonage VID/PID, upload sketch `hardware/microcontroleur/arduino.ino`.
  - *User/System* – infos licence, HWID, charge CPU, FPS capture.
- **Overlay avancé** : fenêtrage frameless toujours-on-top, hints transparents, support multi-color palette & blinking.
- **Journaux & support** : `logs/activity/` pour observer la calibration, `logs/crash/` pour analyser les exceptions, export simple lors d’une demande de support.

## Comparatif express

| Solution | Saobot | Colorbots classiques |
| --- | --- | --- |
| UI & UX | Dashboard complet, thèmes clair/sombre, overlay custom | Interfaces minimalistes, options limitées |
| Spoofing | Gestion Arduino intégrée + firmware prêt | Outils tiers à configurer soi-même |
| Support | Boutons dédiés vers Discord/boutique, logs structurés | Généralement Discord-only sans diagnostics |
| Packaging | `.exe` PyInstaller signé d’un icon Saobot | Scripts bruts nécessitant Python manuel |

## Acheter & activer Saobot

1. Rendez-vous sur **[saobot.shop](https://saobot.shop)** pour sélectionner une formule.
2. Le paiement valide immédiatement une clé liée à votre HWID.
3. Téléchargez la dernière release (`dist/Saobot.exe`) ou exécutez `python main.py` si vous préférez les sources.
4. Saisissez la clé dans le portail d’accès. L’application affiche alors les informations de licence, la date d’expiration et les liens support.

> Besoin d’assistance ? Cliquez sur **Support Discord** dans la fenêtre de login pour ouvrir directement un ticket.

## Installation développeur

```powershell
git clone https://github.com/<votre-org>/saobot.git
cd saobot
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r documentation/requirements.txt
python main.py
```

- `configuration/settings.ini` est généré automatiquement.
- Le firmware Arduino se trouve dans `microcontroleur/arduino.ino` (Leonardo recommandé).
- Pour générer l’exécutable Windows : `pyinstaller main.spec` → sortie `dist/Saobot.exe` (~100 Mo).

## Utilisation rapide

1. Lancer Saobot (`Saobot.exe` ou `python main.py`).
2. Entrer la licence ➜ accès accordé.
3. Configurer les modules nécessaires (Aimbot/Triggerbot/Anti-recoil/FOV/Spoofing).
4. Cliquer **Lancer le bot** pour démarrer la capture et les actions automatisées.
5. Utiliser l’onglet Spoofing pour flasher ou cloner un périphérique si nécessaire.

## Prérequis techniques

- Windows 10/11 64 bits.
- GPU compatible DirectX 11 (dxcam/d3dshot).
- Python 3.10+ pour les profils développeurs.
- Arduino Leonardo (ou compatible) pour le spoofing USB.
- Connexion Internet pour la vérification de licence et le téléchargement d’outils (arduino-cli, dépendances pip).

## Architecture du dépôt

```
COLORBOT VALORANT MAIN GUI/
├─ assets/                 # icônes, branding (saobot.ico)
├─ src/
│  ├─ application/         # GUI, capture, modules bot, spoofing
│  └─ configuration/       # settings, parsers, helpers
├─ microcontroleur/        # firmware Arduino + licence
├─ documentation/          # requirements, guides bilingues
├─ build/, dist/           # artefacts PyInstaller
├─ logs/                   # activity + crash reports
└─ main.py
```

## Support & communauté

- **Site** : [saobot.shop](https://saobot.shop)
- **Discord** : bouton Support dans l’écran de connexion ou utilisez le lien imprimé dans l’app.
- **Logs** : joignez `logs/activity/` + `logs/crash/` lors d’un ticket pour accélérer le diagnostic.

## Avertissements juridiques

- Saobot est fourni « tel quel » pour un usage éducatif/démonstratif. Aucune garantie quant aux conséquences en jeu ou sur votre compte.
- L’utilisation peut violer les CGU de Valorant ou de Riot Games. Vous êtes seul responsable des risques encourus (bannissement, sanctions, pertes de compte, etc.).
- Revente, rétro-ingénierie, redistribution ou partage de licence interdits sans accord écrit.
- Toute tentative de contournement ou de duplication entraîne la révocation immédiate de la licence sans remboursement.

---

© 2025 – Saobot. Tous droits réservés. Toute diffusion hors contexte éducatif nécessite notre accord écrit.

