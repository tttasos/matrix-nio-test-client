# MatrixClientAndOrBot

MatrixClientAndBotTest is a Python-based client or perhaps bot, designed to interact with the [Matrix protocol](https://matrix.org/).

## Features

- Connect to Matrix homeservers
- Send and receive messages
- Handle events (e.g., new messages, invites)

## Requirements

- Python 3.13+
- A Matrix account and access to a homeserver
- The following Python packages:
  - [`matrix-nio`](https://github.com/poljar/matrix-nio) (used for Matrix API interactions, it will install whatever else is needed)

Install dependencies:

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install matrix-nio
```

## Configuration

Before running the bot, configure your credentials:

```bash
cp config.example.json config.json
```

Then edit `config.json` with your Matrix username, password or access token, and homeserver URL.

Example `config.json`:

```json
{
  "homeserver": "https://matrix.org",
  "user_id": "@yourbot:matrix.org",
  "access_token": "YOUR_ACCESS_TOKEN",
  "device_id": "YOUR_DEVICE_ID",
  "store_path": "./store"
}
```

> ⚠️ Keep your access token secure. Do not commit it to version control.

## Usage

Run the bot with:

```bash
python main.py
```

This will log in, sync with the server, and begin listening for events.

## Project Structure

```
matrixbot/
│
├── main.py               # Entry point
├── config.json           # Configuration file
├── handlers/             # Event handler modules
│   └── message_handler.py
├── utils/                # Utility modules
├── store/                # Encrypted store for sync tokens and keys
└── README.md             # Project documentation
```

## Example

The bot will do its work.... Stay tuned.... :)

## Contributing

Contributions are welcome! Please submit issues and pull requests via GitHub.

1. Fork the repo
2. Create a new branch (`git checkout -b feature-xyz`)
3. Commit your changes
4. Push and open a pull request

## License

MIT License

---

© 2025 Tasos Kikilis
