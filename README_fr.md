<!--
N.B.: Ce README a été automatiquement généré par https://github.com/YunoHost/apps/tree/master/tools/readme_generator
Il ne doit PAS être modifié à la main.
-->

# FlareSolverr pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/flaresolverr.svg)](https://ci-apps.yunohost.org/ci/apps/flaresolverr/) ![Statut du fonctionnement](https://ci-apps.yunohost.org/ci/badges/flaresolverr.status.svg) ![Statut de maintenance](https://ci-apps.yunohost.org/ci/badges/flaresolverr.maintain.svg)
[![Installer FlareSolverr avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=flaresolverr)

*[Read this README in english.](./README.md)*

> *Ce package vous permet d'installer FlareSolverr rapidement et simplement sur un serveur YunoHost.
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

FlareSolverr est un serveur proxy permettant de contourner les protections Cloudflare et DDoS-GUARD. Il démarre un serveur proxy qui attend les requêtes utilisateur en état d'inactivité, consommant peu de ressources. Lorsqu'une requête arrive, il utilise un navigateur headless (Chromium) pour ouvrir l'URL avec les paramètres fournis et attend que le défi Cloudflare soit résolu (ou que le délai expire). Le code HTML et les cookies sont renvoyés à l'utilisateur, et ces cookies peuvent être utilisés pour contourner Cloudflare avec d'autres clients HTTP.

### Fonctionnalités

- Contournement automatique des défis Cloudflare
- Support de la configuration proxy
- Interface API REST
- Faible consommation de ressources au repos
- Navigateur Chromium headless inclus

**Version incluse :** 3.3.21~ynh1

## Capture d'écran

![Capture d'écran de FlareSolverr](./doc/screenshots/screenshot.jpg)

## Documentations et ressources

* Dépôt de code officiel de l'app : <https://github.com/FlareSolverr/FlareSolverr>
* Documentation YunoHost pour cette app : <https://yunohost.org/app_flaresolverr>
* Signaler un bug : <https://github.com/Wiwileborne/flaresolverr_ynh/issues>

## Mainteneurs

Ce package est maintenu par **Wiwileborne**.

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/Wiwileborne/flaresolverr_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.

``` bash
sudo yunohost app install https://github.com/Wiwileborne/flaresolverr_ynh/tree/testing --debug
ou
sudo yunohost app upgrade flaresolverr -u https://github.com/Wiwileborne/flaresolverr_ynh/tree/testing --debug
```

**Plus d'infos sur le packaging d'applications :** <https://yunohost.org/packaging_apps>
