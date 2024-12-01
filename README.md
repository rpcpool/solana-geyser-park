# Geyser Park

**This is not an offical or endorsed list and is not affiliated with Solana Labs or the Solana Foundation in any way.**

The Solana Geyser interface is a handy way to access both account writes, blocks and (in 1.9) transactions as they are processed by the validator.

This is a list of various Geyser plugins available. Feel free to send a PR with your own.

For more info about the Geyser interface: https://docs.solana.com/developing/plugins/geyser-plugins

## Geyser Plugins

 * [Postgres](https://github.com/solana-labs/solana-accountsdb-plugin-postgres): The OG plugin by the developers of the Geyser interface in Solana team, supports inserting into postgres.
 * [gRPC](https://github.com/ckamm/solana-accountsdb-connector): A generic gRPC interface along with a sample connector for writing the gRPC stream to Postgres. By the Mango team.
 * [RabbitMQ](https://github.com/holaplex/indexer-geyser-plugin): A RabbitMQ writer. By the Holaplex team. Now separated from the rest of the indexer.
 * [Kafka](https://github.com/Blockdaemon/solana-accountsdb-plugin-kafka): A Geyser plugin to publish to Kafka. By the Blockdaemon team.
 * [Bigtable](https://github.com/lijunwangs/solana-accountsdb-plugin-bigtable): WIP progress (non production ready) for Google Big Table. By the Solana team.
 * [gRPC](https://github.com/rpcpool/solana-geyser-grpc): Replacement for websockets with gRPC bidirectional streaming. By Triton One.

## Geyser Related

 * [Solana Postgres RPC server](https://github.com/lijunwangs/solana-postgres-rpc-server): A server to respond to RPC requests via Postgres data written by the Postgres plugin.
 * [gRPC connector](https://github.com/ckamm/solana-accountsdb-connector/tree/master/connector-mango): A connector that connects to gRPC plugin to parse data received.

## An actual Geyser

<img src="https://user-images.githubusercontent.com/5172293/158663966-af7fedb8-e581-4176-8191-33884ff3389a.png" height="300"/>
