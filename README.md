# Bitcoin Knots for StartOS, in Kilombino's registry

The official StartOS package of **Bitcoin Knots 29.5.1** (`bitcoind`, flavor
`#knots:29.5.1:2`), a full node that follows the BLAKE2b chain, offered in
[registry.kilombino.com](https://registry.kilombino.com) beside Kilombino's
other apps (Lightning XBT, DATUM, MRR Command Center).

**Nothing in the software is changed.** It is the `.s9pk` that Horizon publishes in
[Horizon-btc/knots-startos](https://github.com/Horizon-btc/knots-startos/releases/tag/v29.5.1.knots20260508)
and lists in the start9.mempool.guide registry, checked against its published
SHA-256 (`30b4d7f4…3595`) and Horizon's GPG signature (key `FA651CDD56832225FEA35B4EA1E0862F6A7AC6AE`) and re-signed with Kilombino's key, so StartOS
does not ask you to trust another signer. The only edits are in the manifest: `packageRepo`
(capitalisation of Horizon's repository URL) and the release notes (Horizon's
one line, expanded with the consensus change and the fixes in Knots' own
release notes); editing it re-signs it. Needs StartOS 0.4.2 or later.
I2P is now Horizon's separate, optional `i2pd` package.

All credit to Bitcoin Knots (Luke Dashjr and contributors,
[bitcoinknots/bitcoin](https://github.com/bitcoinknots/bitcoin)) and to
Horizon for the package. Licence: MIT, as upstream.

## Releases

- `v29.5.1_2`: `bitcoind.s9pk` (aarch64, riscv64, x86_64), re-signed from
  Horizon's v29.5.1.knots20260508 (Bitcoin Knots 29.5.1, StartOS SDK 4.1.0).
  Consensus: BIP110's BAN_ANNEX now also applies to spends of outputs created
  before block 961640 (no annex was used since 961640, so no reorg);
  CVE-2026-117348 fixed; spam filter improvements.

- `v29.5_3`: `bitcoind.s9pk` (aarch64, riscv64, x86_64), re-signed from
  Horizon's v29.5.knots20260508 (Bitcoin Knots 29.5, StartOS SDK 4.0.0).

- `v29.4.3_1`: `bitcoind.s9pk` (aarch64, riscv64, x86_64), re-signed from
  Horizon's v29.4.3.knots20260508.
