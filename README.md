

[![license](https://img.shields.io/github/license/NextDom/plugin-ONVIF.svg)](./LICENSE) [![GitHub contributors](https://img.shields.io/github/contributors/NextDom/plugin-ONVIF.svg)](../../graphs/contributors) [![GitHub release](https://img.shields.io/github/release/NextDom/plugin-ONVIF.svg)](../../releases) [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/_USERNAME) [![Waffle.io - Columns and their card count](https://badge.waffle.io/NextDom/plugin-ONVIF.svg?columns=all)](https://waffle.io/NextDom/plugin-ONVIF) [![Join the chat at https://gitter.im/NextDom/Developpement](https://badges.gitter.im/NextDom/plugin-ONVIF.svg)](https://gitter.im/NextDom/plugin-ONVIF?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

### Master: [![Build Status](https://travis-ci.org/NextDom/plugin-ONVIF.svg?branch=master)](https://travis-ci.org/NextDom/plugin-ONVIF)  [![Coverage Status](https://coveralls.io/repos/github/NextDom/plugin-ONVIF/badge.svg?branch=master)](https://coveralls.io/github/NextDom/plugin-ONVIF?branch=master)

### Develop: [![Build Status](https://travis-ci.org/NextDom/plugin-ONVIF.svg?branch=develop)](https://travis-ci.org/NextDom/plugin-ONVIF)  [![Coverage Status](https://coveralls.io/repos/github/NextDom/plugin-ONVIF/badge.svg?branch=develop)](https://coveralls.io/github/NextDom/plugin-ONVIF?branch=develop)

# Présentation:

Ce plugin permet de controler les caméras supportant le protocole ONVIF. 

Dependances requises:

`npm install onvif`

`npm install minimist`

# Les commandes supportées:

## La détection de caméras:

Le plugin propose de détécter les caméra supportant le protocole ONVIF, en créant un equipement par caméra détéctée comportant les adresses de ces differentes caméras par exemple dans un cas de figure avec deux caméras:

```
Nombre de camera = 2

Adresse1: https://192.168.1.20:951/onvif/device_service

Adresse2: https://192.168.1.28:4651/onvif/device_service
```
On aurait deux équipements générés avec l'url déjà renseignée.

## Actions supportées dans Jeedom:

* GoToHome : Permet d'aller à la position par défaut de la caméra, cette position est modifiable.
* GoToPreset : Permet à la caméra d'aller à une position prédéfini sous la forme de preset PTZ par l'utilisateur.
* RelativeMove : Permet à la caméra d'effectuer un mouvement relatif par rapport à la position initiale.
* SetPreset : Créer un preset au niveau de la position actuelle de la caméra, ce preset peut être appelé avec la fonction GoToPreset.
* RemovePreset : Supprime un preset enregistré sur la caméra.
* SetImageSettings : Permet de controler les paramètres de l'image a travers quatres fonctions:
  * Luminosité
  * Contraste
  * Saturation
  * Netteté
* AbsoluteMove : Déplace la caméra à des coordonnées fixés.
* Reboot : Redémare la caméra 5 secondes après la requête

## Infos supportées dans Jeedom:

* GetPreset 
* GetScope
* GetStatus
* GetDate
* GetDeviceInfo
* GetHost
* GetImageSettings
* GetNodes 
* GetProfile
* GetReplayURL
* GetStreamURL
* GetSnapshotURL

# FORUM
[Forum Nextdom](https://www.nextdom.org/forum/plugin-onvif)

# Documentation du plugin:
[![Read the Docs](https://img.shields.io/readthedocs/pip.svg)](docs/fr_FR/presentation.md)
[présentation](docs/fr_FR/presentation.md) [configuration](docs/fr_FR/configuration.md) [faq](docs/fr_FR/faq.md) [changelog](docs/fr_FR/changelog.md)

# Documentation complète:

[![Read the Docs](plugin_info/ONVIF_icon.png)](https://NextDom.github.io/plugin-ONVIF)


[![Support via PayPal](https://cdn.rawgit.com/twolfson/paypal-github-button/1.0.0/dist/button.svg)](https://www.paypal.me/_USERNAME/)

