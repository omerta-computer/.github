<p align="center"><img src="https://raw.githubusercontent.com/omerta-computer/.github/main/profile/assets/banner.png" width="100%" alt="OMERTA"></p>

# OMERTA

<p>
  <a href="https://omerta.computer"><img src="https://img.shields.io/badge/website-omerta.computer-111111" alt="Website"></a>
  <a href="https://x.com/omertachain"><img src="https://img.shields.io/badge/X-%40omertachain-111111" alt="X · @omertachain"></a>
  <a href="https://github.com/omerta-computer/omerta"><img src="https://img.shields.io/badge/source-omerta-111111" alt="Source repository"></a>
  <a href="https://github.com/omerta-computer/omerta/blob/main/docs/whitepaper.md"><img src="https://img.shields.io/badge/docs-whitepaper-111111" alt="Whitepaper"></a>
  <a href="https://github.com/omerta-computer/omerta/blob/main/docs/API.md"><img src="https://img.shields.io/badge/SDK-API-111111" alt="SDK reference"></a>
  <a href="https://github.com/omerta-computer/omerta/blob/main/docs/official-tools.md"><img src="https://img.shields.io/badge/CLI-checks-111111" alt="Stock CLI checks"></a>
  <a href="https://github.com/omerta-computer/omerta/blob/main/VERIFY.md"><img src="https://img.shields.io/badge/verification-results-111111" alt="Verification"></a>
</p>

OMERTA runs a Solana-compatible chain for confidential transfers. Its four validators run Agave. Token-2022 handles the main asset, and the native ZK ElGamal Proof program verifies transfers.

## What a transfer reveals

A transfer records the sender, recipient, mint, fee payer and slot. The amount and each sealed balance are ciphertext. The owner derives the keys locally and can read the balance with the wallet or the stock `spl-token` CLI. The mint has no auditor key.

The wallet seals new accounts and disables public credits. The account owner can later change that setting. Minting, deposits, withdrawals and native gas fees have publicly visible amounts.

## Run the checks

The `omerta` repository contains the TypeScript SDK, the patch against Agave, the genesis program manifest and a proof benchmark. The SDK tests run offline. The CLI guide also shows how to inspect an account and compare public and confidential transfers on a running network.

## Network assets

The current network uses `TEST` for confidential transfers and `GAS` for fees. The proposed $OMERTA gas and staking transition is a separate stage.
