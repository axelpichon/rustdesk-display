# RustDesk Display

Pendant une session RustDesk entrante, éteint les écrans physiques du PC Windows et active un écran virtuel à la résolution de l'appareil qui se connecte. Les écrans physiques sont rallumés à la fin de la session.

Ce dépôt ne contient que les versions publiées.

## Installation

Télécharger `rustdesk-display.exe` depuis la [dernière release](https://github.com/axelpichon/rustdesk-display/releases/latest), double-cliquer dessus et accepter la demande d'autorisation administrateur. L'exécutable embarque le pilote d'écran virtuel ([Virtual Display Driver](https://github.com/VirtualDrivers/Virtual-Display-Driver), licence MIT) et s'installe dans `C:\Program Files\RustDeskDisplay`. Désinstallation : **Paramètres > Applications installées**.

L'icône près de l'horloge permet de choisir la résolution et l'échelle de chaque appareil.

## Mise à jour

Automatique : le service vérifie les releases de ce dépôt toutes les 6 h et installe la nouvelle version dès qu'aucune session RustDesk n'est en cours. Pour forcer : `rustdesk-display.exe update`. Pour désactiver : `"autoUpdate": false` dans `C:\ProgramData\RustDeskDisplay\config.json`.