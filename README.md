{\rtf1\ansi\ansicpg1252\cocoartf2821
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fnil\fcharset0 .SFNS-Heavy;}
{\colortbl;\red255\green255\blue255;\red14\green14\blue14;}
{\*\expandedcolortbl;;\cssrgb\c6700\c6700\c6700;}
\paperw11900\paperh16840\margl1440\margr1440\vieww35800\viewh19700\viewkind0
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\sl324\slmult1\pardirnatural\partightenfactor0

\f0\b\fs26 \cf2 # Yoshi Animation Project - Super Mario World 71438\
\
Ce projet ESPHome anime Yoshi \'e0 l'aide de :\
- Deux servos : un pour tirer la langue, un pour faire courir Yoshi.\
- 14 LEDs WS2812 pour des effets lumineux.\
- Un module DFPlayer Mini pour jouer des sons sp\'e9cifiques.\
\
## Fonctionnalit\'e9s\
- **Servo pour la langue** : mouvement fluide de 0\'b0 \'e0 180\'b0.\
- **Servo pour courir** : va-et-vient continu pour simuler la course.\
- **Effets lumineux** : animations synchronis\'e9es avec 14 LEDs WS2812.\
- **Son** : sons personnalis\'e9s jou\'e9s via DFPlayer Mini.\
\
## Mat\'e9riel requis\
- ESP32\
- 2 Servos (1 classique, 1 \'e0 rotation continue)\
- 14 LEDs WS2812\
- DFPlayer Mini + haut-parleur\
- Set LEGO Super Mario World 71438\
- Boutons pour d\'e9clencher les animations\
\
## Connexions\
| Composant         | GPIO ESP32 | Remarque              |\
|--------------------|------------|-----------------------|\
| Servo langue       | GPIO16     | Contr\'f4le classique    |\
| Servo courir       | GPIO18     | Rotation continue     |\
| LEDs WS2812        | GPIO21     | Alimentation 5V       |\
| DFPlayer Mini RX   | GPIO1      | Communication s\'e9rie   |\
| DFPlayer Mini TX   | GPIO3      | Communication s\'e9rie   |\
| Bouton langue      | GPIO26     | Input avec pull-up    |\
| Bouton courir      | GPIO23     | Input avec pull-up    |\
\
## Installation\
1. T\'e9l\'e9chargez les fichiers du projet.\
2. Pr\'e9parez votre ESPHome en suivant [ce guide](https://esphome.io/guides/getting_started.html).\
3. Flashez `esphome_config.yaml` sur votre ESP32.\
4. Connectez les composants selon le sch\'e9ma.\
\
## D\'e9monstration\
![LED Animation](assets/led_effect_demo.mp4)\
\
## Sch\'e9ma des connexions\
![Sch\'e9ma](assets/schema_diagram.png)\
\
## Contribuer\
Voir [CONTRIBUTING.md](CONTRIBUTING.md).}