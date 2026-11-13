# Bitcoin Knots for StartOS, in Kilombino's registry

The official StartOS package of **Bitcoin Knots 29.5** (`bitcoind`, flavor
`#knots:29.5.0:3`), a full node that follows the BLAKE2b chain, offered in
[registry.kilombino.com](https://registry.kilombino.com) beside Kilombino's
other apps (Lightning XBT, DATUM, MRR Command Center).

**Nothing in it is changed.** It is the `.s9pk` that Horizon publishes in
[Horizon-btc/knots-startos](https://github.com/Horizon-btc/knots-startos/releases/tag/v29.5.knots20260508)
and lists in the start9.mempool.guide registry, checked against its published
SHA-256 (`017ed246…5e3d`) and Horizon's GPG signature (key `FA651CDD56832225FEA35B4EA1E0862F6A7AC6AE`) and re-signed with Kilombino's key, so StartOS
does not ask you to trust another signer. The only edit is the manifest's
`packageRepo` (capitalisation of Horizon's repository URL), which re-signs it. Needs StartOS 0.4.1 or later.

All credit to Bitcoin Knots (Luke Dashjr and contributors,
[bitcoinknots/bitcoin](https://github.com/bitcoinknots/bitcoin)) and to
Horizon for the package. Licence: MIT, as upstream.

## Releases

- `v29.5_3`: `bitcoind.s9pk` (aarch64, riscv64, x86_64), re-signed from
  Horizon's v29.5.knots20260508 (Bitcoin Knots 29.5, StartOS SDK 4.0.0).

- `v29.4.3_1`: `bitcoind.s9pk` (aarch64, riscv64, x86_64), re-signed from
  Horizon's v29.4.3.knots20260508.
