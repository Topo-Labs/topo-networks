# Topo Chain genesis blob and waypoint for different networks

- `devnet/`: Developer testnet, upgraded weekly on Thursday from main branch, data will be wiped when upgrade.
- `testnet/`: Topo Chain stable testnet, data will be persisted during upgrades. 
- `mainnet/`: Topo Chain Mainnet

# Run full node

- Start full node with `devnet/` genesis blob and waypoint:

```bash
./bin/aptos-node -f ./devnet/full_node.yaml
```