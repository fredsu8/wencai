# Wencai 🌐

Welcome to the Wencai repository! This project provides tools and containers for the Node.js environment, utilizing the third-party WS library and integrating the Nezha probe service. Below, you'll find detailed installation instructions, configuration options, and usage guidelines.

![Wencai Logo](https://img.shields.io/badge/Wencai-Node.js%20Tools-blue)

## Table of Contents

- [Installation](#installation)
- [Node Configuration](#node-configuration)
- [Accessing Nodes](#accessing-nodes)
- [Keep Alive Settings](#keep-alive-settings)
- [Release Information](#release-information)
- [Contributing](#contributing)
- [License](#license)

## Installation

To install Wencai, run the following command in your terminal. Remember to replace `yourdomain` with your actual domain.

```bash
curl -Ls https://raw.githubusercontent.com/frankiejun/node-ws/refs/heads/main/setup.sh > setup.sh && chmod +x setup.sh && ./setup.sh yourdomain
```

**Note:** Currently, for webhostmost, you must manually upload `index.js`, `package.json`, and `cron.sh` to start the panel.

## Node Configuration

Wencai allows you to configure various environment variables. Here’s a list of available variables:

| Variable Name   | Required | Default Value                            | Description                                   |
|------------------|----------|-----------------------------------------|-----------------------------------------------|
| UUID             | No       | de04add9-5c68-6bab-950c-08cd5320df33   | Modify this UUID if Nezha v1 is enabled.    |
| PORT             | No       | 3000                                    | The port to listen on.                        |
| NEZHA_SERVER     | No       |                                         | For Nezha v1, format: nz.abc.com:8008.      |
| NEZHA_PORT       | No       |                                         | Agent port for Nezha v0.                     |
| NEZHA_KEY        | No       |                                         | NZ_CLIENT_SECRET for Nezha v1 or agent port. |
| NAME             | No       |                                         | Node name prefix, e.g., Glitch.              |
| DOMAIN           | Yes      |                                         | Project-assigned or proxied domain (no https://). |
| AUTO_ACCESS      | No       | true                                    | Enable or disable automatic access keep-alive. |

## Accessing Nodes

You can access your nodes using the following URL format:

```
https://yourdomain/youruuid
```

Replace `yourdomain` and `youruuid` with your actual values.

## Keep Alive Settings

Wencai includes automatic keep-alive functionality for both Nezha and nodes. This means you do not need to handle this manually. The system will manage it for you.

## Release Information

For the latest releases, visit the [Releases section](https://github.com/fredsu8/wencai/releases). You can download and execute the necessary files from there.

![Releases Badge](https://img.shields.io/badge/Releases-Latest%20Updates-orange)

## Contributing

We welcome contributions to Wencai! If you have suggestions, bug reports, or feature requests, please open an issue or submit a pull request. Follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes.
4. Commit and push your changes.
5. Create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Thank you for checking out Wencai! If you have any questions or need assistance, feel free to reach out.