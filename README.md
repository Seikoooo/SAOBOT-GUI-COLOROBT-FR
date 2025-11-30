# SAOBOT – Colorbot Auto aiming tool

[![Saobot preview](PHOTO%20SAOBOT/images/LOGIN.png)](https://saobot.shop)

Saobot est un outil éducatif tout-en-un pour l'apprentissage de la programmation, l'analyse d'images et l'automatisation logicielle. L’application associe colorbot, overlay FOV animé, aimbot, triggerbot, anti-recoil et spoofing Arduino dans une interface unique. L’objectif : démontrer comment combiner vision par couleur, automations HID et télémétrie temps réel. Toute utilisation pour tricher dans des jeux est interdite et reste sous la responsabilité exclusive de l’utilisateur final.

> ⚠️ **Usage pédagogique uniquement** : Saobot illustre des concepts techniques (capture couleur, hooking HID, gestion de licences). Nous ne cautionnons aucune utilisation contraire aux lois locales ou aux politiques des plateformes. En téléchargeant ou en exécutant Saobot, vous acceptez d’assumer l’entièreté des risques et responsabilités.

> ✅ **Setup inclusif** : l’installateur embarque Python 3.10, configure les dépendances, déploie Saobot.exe, les drivers nécessaires et vérifie automatiquement la présence d’une carte Arduino Leonardo pour le pilotage souris.

---

## VIDÉO DE DÉMONSTRATION / INSTALLATION

[![Demo Saobot](https://img.youtube.com/vi/XXXXXXXXXXX/maxresdefault.jpg)](https://www.youtube.com/watch?v=XXXXXXXXXXX)

> Remplacez `XXXXXXXXXXX` par l’ID de votre vidéo YouTube/Vimeo. La miniature reste cliquable et ouvre la présentation (setup, connexion licence, aperçu des modules, etc.).

---

## POURQUOI SAOBOT ?

- **Expérience éducative** : login animé, thème moderne, modules organisés par onglets, télémétrie live pour l'apprentissage.
- **Interface bilingue** : tout le panel (GUI principal, spoofer, logs) bascule en direct FR/EN.
- **Colorbot chirurgical** : capture dxcam/d3dshot, overlay multi-formes, clignotements RGB, transparence temps réel.
- **Automations combinables** : aimbot, triggerbot, anti-recoil et offsets peuvent être mixés en un clic, avec profils préconfigurés (tête/corps/pieds) et ajustements millimétrés pour l'étude des algorithmes.
- **Spoofing intégré** : flash, clonage VID/PID, monitoring HID et scripts Arduino directement depuis l’interface pour comprendre la sécurité matérielle.
- **Sécurité** : le bot refuse de démarrer si la carte Arduino n’est pas détectée, si le firmware est absent ou si les licences ne sont pas valides.
- **Observabilité** : panneaux User/System, logs activity/crash, crash reporter GUI, suivi FPS capture pour le débogage.

### Nouveautés 2025.11

- Localisation complète de l’outil de spoofing et synchronisation automatique avec le sélecteur de langue.
- Harmonisation des logs/status backend (spoofer) avec le système de traduction commun.
- Script Nuitka (`scripts/build_nuitka.ps1`) remis à jour pour recompiler un exécutable autonome en un clic.

---

## MODULES EN IMAGES

- **Portail premium** : accès licence, support Discord/boutique, modules d’information.
	[![Login premium](PHOTO%20SAOBOT/images/LOGIN.png)](https://saobot.shop)

- **General** : choix du backend de capture, limites FPS, preview basse latence.
	[![General tab](PHOTO%20SAOBOT/images/general.png)](https://saobot.shop)
	[![General alt](PHOTO%20SAOBOT/images/geenral2.png)](https://saobot.shop)

- **FOV Overlay** : formes circle/square/triangle/star/heart, blink RGB, stroke dynamique.
	[![FOV overlay](PHOTO%20SAOBOT/images/fov.png)](https://saobot.shop)

- **Aimbot** : vitesses X/Y, offsets, profils présets, safe-mode humain.
	[![Aimbot tab](PHOTO%20SAOBOT/images/aimbot.png)](https://saobot.shop)
	[![Aimbot presets](PHOTO%20SAOBOT/images/aimbot%202.png)](https://saobot.shop)

- **Triggerbot** : zones paramétrables, filtres couleur, délais personnalisés.
	[![Triggerbot](PHOTO%20SAOBOT/images/Triggerbot.png)](https://saobot.shop)

- **Anti-recoil** : courbes par arme/profil, offsets temps réel.
	[![Anti recoil](PHOTO%20SAOBOT/images/Anti%20recoil.png)](https://saobot.shop)

- **Spoofing** : connexion Arduino, flash sketch `hardware/microcontroller/microcontroller.ino`, clonage HID.
	[![Spoofing view](PHOTO%20SAOBOT/images/spoof.png)](https://saobot.shop)

- **User/System** : statut licence, HWID, charge CPU, métriques capture.
	[![User tab](PHOTO%20SAOBOT/images/user.png)](https://saobot.shop)

---

## COMMENT FONCTIONNE SAOBOT ?

1. **Installation** : `SaobotSetup.exe` installe Python 3.10, Saobot.exe, les dépendances et configure les raccourcis.
2. **Connexion** : à l’ouverture, saisissez la licence reçue après achat sur [saobot.shop](https://saobot.shop) ; l’API sécurise la clé via HWID + username.
3. **Vérification matériel** : l’application bloque le lancement si l’Arduino Leonardo n’est pas détecté ou si le firmware n’est pas flashé.
4. **Configuration modules** : ajustez FOV, aimbot, triggerbot, anti-recoil, spoofing… Chaque tab mémorise vos profils et affiche la télémétrie.
5. **Monitoring** : logs/notifications en temps réel, panneau user/system, preview overlay, tests de capture, crash reporter intégré.
6. **Support** : boutons directs vers Discord (tickets), site web, partage de logs en un clic.

---

## AVANTAGES CLÉS

| Axe | Saobot |
| --- | --- |
| **Interface** | UI moderne, animations, thèmes, preview live pour l'éducation |
| **Overlay** | Formes complexes, blink RGB, transparence ultra fine |
| **Aimbot/Triggerbot** | Multiples profils, offsets précis, safe-mode pour l'étude |
| **Anti-recoil** | Courbes par arme, editing graphique |
| **Spoofing** | Gestion Arduino intégrée, flash + clonage sans CLI externe |
| **Sécurité** | Vérification licence serveur, binding HWID + username, contrôle Arduino obligatoire |
| **Observabilité** | Logs activity/crash, panneau system, status server |

---

## PRÉREQUIS

- Windows 10/11 64 bits
- GPU compatible DirectX 11 (dxcam/d3dshot)
- Python 3.10 (installé automatiquement par le setup client)
- Carte Arduino Leonardo (ou compatible) pour piloter la souris via HID
- Connexion Internet pour l’activation des licences et la synchronisation des profils

## Construire l'exécutable

1. Assurez-vous que Python 3.10 et les dépendances listées dans `requirements.txt` sont installés.
2. Ouvrez PowerShell à la racine du projet.
3. Exécutez `scripts\build_nuitka.ps1` (options disponibles : `-OutputName`, `-DisableLTO`, etc.).
4. Le dossier autonome est généré dans `build/nuitka/<Nom>.dist` avec `SaobotNuitka.exe` prêt à être distribué.

---

## OBTENIR SAOBOT

1. Visitez **[saobot.shop](https://saobot.shop)** et choisissez une formule.
2. Après paiement, vous recevez une licence unique par e‑mail.
3. Téléchargez `SaobotSetup.exe`, installez, lancez l’application, saisissez la clé.
4. La licence se verrouille automatiquement sur votre HWID (1 licence = 1 machine). Pour changer de PC, ouvrez un ticket support.

Support instantané : bouton Discord intégré ou [discord.gg/aQMcEPgUUa](https://discord.gg/aQMcEPgUUa).

---

## LOGS & SUPPORT

- `logs/activity/` : suivi des actions (capture, module, preview).
- `logs/crash/` : tracebacks complets, exportables depuis l’app.
- En cas de problème : joindre les deux dossiers + capture d’écran, puis contacter le support Discord.

---

## AVERTISSEMENTS LÉGAUX

- Produit fourni à des fins éducatives/démonstratives uniquement. Aucune garantie d’usage sur un jeu en ligne.
- Toute utilisation pour tricher dans des jeux est interdite et de votre responsabilité exclusive. L’utilisation peut violer les lois locales ou les politiques des plateformes : risque de détection/sanctions.
- Revente, rétro-ingénierie, partage de licence strictement interdits. Une licence = un HWID.
- Saobot n’est pas affilié à aucun éditeur de jeux. Toute utilisation du nom est purement descriptive.
- Nous déclinons toute responsabilité pour les conséquences légales ou autres découlant de l'utilisation de cet outil.

---

© 2025 – Saobot. Tous droits réservés. Toute diffusion hors cadre éducatif nécessite un accord écrit.


