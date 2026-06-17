# Topo Chain genesis blob and waypoint for different networks

- `devnet/`: Developer testnet, upgraded weekly on Thursday from main branch, data will be wiped when upgrade.
- `testnet/`: Topo Chain stable testnet, data will be persisted during upgrades. 
- `mainnet/`: Topo Chain Mainnet

# Run full node

- Start full node with `devnet/` genesis blob and waypoint:

```bash
./bin/aptos-node -f ./devnet/full_node.yaml
```

- `devnet/full_node.yaml` and `devnet/full_node_example.yaml` are `public` fullnode configurations and do not depend on a private `vfn` network.
- `devnet/full_node_example.yaml` includes a local-path example, `indexer_table_info`, and `indexer_grpc` configuration.
- Docker Compose exposes:
  - Aptos API at `127.0.0.1:8080`
  - Indexer gRPC at `127.0.0.1:30041`
