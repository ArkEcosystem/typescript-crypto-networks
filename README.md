# ARK TypeScript Crypto - Network Configurations

<p align="center">
    <img src="./banner.png" />
</p>

> Network Configurations for the ARK Blockchain. Developed for TypeScript.

## Installation

Requires [Node.js](https://nodejs.org) 24 or later.

```bash
npm install @arkecosystem/crypto-networks
```

## Usage

Each network exposes its `exceptions`, `genesisBlock`, `milestones` and `network` configuration.

```ts
import { devnet, mainnet, testnet } from "@arkecosystem/crypto-networks";

mainnet.network.client.symbol; // "Ѧ"
mainnet.milestones[0].height; // 1
```

## Development

The toolchain version is pinned in [.nvmrc](.nvmrc) and used by CI.

```bash
npm ci        # install dependencies
npm run build # compile src to dist
npm run lint  # check formatting
npm run format # apply formatting
```

Network configuration lives in [src/](src/) as plain JSON; each network's `index.ts` only re-exports it.

## Security

If you discover a security vulnerability within this package, please send an e-mail to security@ark.io. All security vulnerabilities will be promptly addressed.

## Credits

This project exists thanks to all the people who [contribute](../../../../contributors).

## License

[MIT](LICENSE) © [ARK Ecosystem](https://ark.io)
