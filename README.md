# besu-clique-gasfree
A sample genesis block data for gas-free private network on Clique (PoA) consensus with Hyperledger Besu.

### Hyperledger Besu

Hyperledger Besu (v24.5.1 or more)

### Quick start

```
% besu --config-file=config.toml
```

That's it. Then the network will start spinning.

### Major Configurations

#### `genesis.json`

* Chain ID: `4649`
* Block production period (sec.): `5`
* Create empty blocks: `TRUE`
* Initial signer account: `0xfe3b557e8fb62b89f4916b721be55ceb828dbd73`

If you want to change the initial signer account into your own one, set it to `extraData` property in `genesis.json`, and update its private key in `besu-data/key` file. For more info: https://besu.hyperledger.org/private-networks/how-to/configure/consensus/clique

#### `config.toml`

* RPC-HTTP host: `127.0.0.1`
* RPC-HTTP port: `4989`
* Data path: `besu-data`
