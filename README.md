# SAOBOT – VALORANT COLORBOT EXPERIENCE

[![Saobot preview](PHOTO%20SAOBOT/images/LOGIN.png)](https://saobot.shop)

Saobot est une expérience premium tout-en-un inspirée de Valorant. L’application associe colorbot, overlay FOV animé, aimbot, triggerbot, anti-recoil et spoofing Arduino dans une interface unique. L’objectif : démontrer comment combiner vision par couleur, automations HID et télémétrie temps réel. Toute utilisation en dehors d’un cadre éducatif reste sous la responsabilité de l’utilisateur final.

> ⚠️ **Usage pédagogique** : Saobot illustre des concepts techniques (capture couleur, hooking HID, gestion de licences). Nous ne cautionnons aucune utilisation contraire aux CGU Riot Games. En téléchargeant ou en exécutant Saobot, vous acceptez d’assumer l’entièreté des risques.

> ✅ **Setup inclusif** : l’installateur embarque Python 3.10, configure les dépendances, déploie Saobot.exe, les drivers nécessaires et vérifie automatiquement la présence d’une carte Arduino Leonardo pour le pilotage souris.

---

## VIDÉO DE DÉMONSTRATION / INSTALLATION

[![Demo Saobot](https://img.youtube.com/vi/XXXXXXXXXXX/maxresdefault.jpg)](https://www.youtube.com/watch?v=XXXXXXXXXXX)

> A REMPLACER.

---

## POURQUOI SAOBOT ?

- **Expérience premium** : login animé, thème inspiré Valorant, modules organisés par onglets, télémétrie live.
- **Colorbot chirurgical** : capture dxcam/d3dshot, overlay multi-formes, clignotements RGB, transparence temps réel.
- **Automations combinables** : aimbot, triggerbot, anti-recoil et offsets peuvent être mixés en un clic, avec profils préconfigurés (tête/corps/pieds) et ajustements millimétrés.
- **Spoofing intégré** : flash, clonage VID/PID, monitoring HID et scripts Arduino directement depuis l’interface.
- **Sécurité** : le bot refuse de démarrer si la carte Arduino n’est pas détectée, si le firmware est absent ou si les licences ne sont pas valides.
- **Observabilité** : panneaux User/System, logs activity/crash, crash reporter GUI, suivi FPS capture.

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
| **Interface** | UI inspirée Valorant, animations, thèmes, preview live |
| **Overlay** | Formes complexes, blink RGB, transparence ultra fine |
| **Aimbot/Triggerbot** | Multiples profils, offsets précis, safe-mode |
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

- Produit fourni à des fins éducatives/démonstratives. Aucune garantie d’usage sur un jeu en ligne.
- L’utilisation peut violer les CGU de Riot Games ou d’autres éditeurs : risque de ban/sanctions.
- Revente, rétro-ingénierie, partage de licence strictement interdits. Une licence = un HWID.
- Saobot n’est pas affilié à Riot Games ou Valorant. Toute utilisation du nom est purement descriptive.

---

© 2025 – Saobot. Tous droits réservés. Toute diffusion hors cadre éducatif ou démonstratif nécessite un accord écrit.

