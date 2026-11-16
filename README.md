# XODE Solochain Releases

Prebuilt binaries and chain specs for the XODE Solochain node. Download them from the
[Releases](https://github.com/D2-Xode/xode-solochain-release/releases) page.

| File | What it is |
|------|------------|
| `xode-solochain-node` | Node binary (Linux x86-64) |
| `xode-mainnet-raw.json` | Raw chain spec for the XODE Solochain mainnet |
| `SHA256SUMS` | Checksums of the files above |

## Quick start

```bash
curl -LO https://github.com/D2-Xode/xode-solochain-release/releases/download/v0.1.0/xode-solochain-node
curl -LO https://github.com/D2-Xode/xode-solochain-release/releases/download/v0.1.0/xode-mainnet-raw.json
curl -LO https://github.com/D2-Xode/xode-solochain-release/releases/download/v0.1.0/SHA256SUMS
sha256sum -c SHA256SUMS
chmod +x xode-solochain-node

./xode-solochain-node \
  --chain ./xode-mainnet-raw.json \
  --base-path ./xode-solochain \
  --name "my-xode-node"
```

For the full setup, including running it as a systemd service, see the
[XODE Solochain Node guide](https://wiki.xode.net/network/xode-solochain-node).
