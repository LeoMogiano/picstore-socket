# Serveur de notification en temps réel

Ce projet est un serveur de notification en temps réel construit avec Express et Socket.IO.

[English](./README.md) | [Español](./README.es.md) | [Français](./README.fr.md) | [日本語](./README.jp.md)

## Prérequis

- Node.js
- npm

## Installation

1. Clonez ce dépôt.
2. Naviguez jusqu'au répertoire du projet.
3. Exécutez `npm install` pour installer les dépendances.

## Utilisation

Pour démarrer le serveur, exécutez `node app.js` dans le terminal. Le serveur écoutera sur le port 3030 ou sur le port spécifié dans votre variable d'environnement `port`.

Le serveur a deux principaux événements Socket.IO :

- `notification` : Cet événement est déclenché lorsqu'un utilisateur émet une notification. Les données de la notification sont préparées pour l'insertion dans la base de données, puis un événement `notification_processed` est émis avec les données de la notification.

- `notification_user` : Cet événement est déclenché lorsqu'un utilisateur émet une notification d'utilisateur. Les données de la notification sont préparées, puis un événement `notification_processed_user` est émis avec les données de la notification.

## Contribution

Les contributions sont les bienvenues. Veuillez ouvrir un ticket (issue) ou une demande de fusion (pull request) pour suggérer des modifications ou des améliorations.

## Licence

Ce projet est sous licence MIT.
