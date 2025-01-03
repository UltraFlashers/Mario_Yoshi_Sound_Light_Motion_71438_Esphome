
Ce projet ESPHome anime Mario & Yoshi l'aide de :
- Deux servos : un pour tirer la langue, un pour faire courir Yoshi.
- 14 LEDs WS2812 pour des effets lumineux.
- Un module DFPlayer Mini pour jouer des sons spécifiques.

![71438LEGO](71438_LEGO.png)

## Fonctionnalités

- **Servo pour la langue** : mouvement fluide de la langue
- **Servo pour courir**    : va-et-vient continu pour simuler la course
- **Effets lumineux**      : animations synchronisés avec 14 LEDs WS2812
- **Son**                  : sons personnalisés joués via DFPlayer Mini

## Matériel requis
- ESP32
- 2 Servos
- 14 LEDs WS2812
- DFPlayer Mini + haut-parleur
- Set LEGO Super Mario World 71438
- Boutons pour déclencher les animations

## Connexions
| Composant          | GPIO ESP32 | Remarque              |
|--------------------|------------|-----------------------|
| Servo langue       | GPIO16     | MG90S classique       |
| Servo courir       | GPIO18     | Servo Standard        |
| LEDs WS2812        | GPIO21     | Alimentation 5V       |
| DFPlayer Mini RX   | GPIO1      | Communication série   |
| DFPlayer Mini TX   | GPIO3      | Communication série   |
| Bouton langue      | GPIO26     | Input avec pull-up    |
| Bouton courir      | GPIO23     | Input avec pull-up    |

## Installation
1. Téléchargez les fichiers du projet.
2. Préparez votre ESPHome en suivant [ce guide](https://esphome.io/guides/getting_started.html).
3. Flashez `esphome_config.yaml` sur votre ESP32.
4. Connectez les composants selon le schéma.

## Démonstration
![LED Animation](assets/led_effect_demo.mp4)

## Schéma des connexions
![Sch\'e9ma](assets/schema_diagram.png)

## License

MIT License
Copyright (c) 2024 UltraFlashers
Permission is hereby granted, free of charge, to any person obtaining a copy...

