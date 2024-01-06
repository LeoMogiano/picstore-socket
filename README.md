# Realtime Notification Server

This project is a real-time notification server built with Express and Socket.IO.

[English](./README.md) | [Español](./README.es.md) | [Français](./README.fr.md) | [日本語](./README.jp.md)

## Requirements

- Node.js
- npm

## Installation

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.

## Usage

To start the server, run `node app.js` in the terminal. The server will begin listening on port 3030 or on the port specified in your `port` environment variable.

The server has two main Socket.IO events:

- `notification`: This event is triggered when a user emits a notification. The notification data is prepared for insertion into the database, and then a `notification_processed` event is emitted with the notification data.

- `notification_user`: This event is triggered when a user emits a user notification. The notification data is prepared, and then a `notification_processed_user` event is emitted with the notification data.

## Contribution

Contributions are welcome. Please open an issue or pull request to suggest changes or improvements.

## License

This project is licensed under the terms of the MIT license.
