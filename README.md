# solana-geyserpark

The Solana Geyser interface is a handy way to access both account writes, blocks and (in 1.9) transactions as they are processed by the validator.

This is a list of various accountsdb plugins available. Feel free to send a PR with your own.

For more info about the accountsdb interface: https://docs.solana.com/developing/plugins/accountsdb_plugin 

## Geyser Plugins

 * [Postgres](https://github.com/solana-labs/solana-accountsdb-plugin-postgres): The OG plugin by the developers of the Geyser interface in Solana team, supports inserting into postgres.
 * [gRPC](https://github.com/ckamm/solana-accountsdb-connector): A generic gRPC interface along with a sample connector for writing the gRPC stream to Postgres. By the Mango team.
 * [RabbitMQ](https://github.com/holaplex/solana-indexer/tree/dev/crates/accountsdb-rabbitmq): A RabbitMQ writer by the Holaplex team.
 * [SQS](https://github.com/rpcpool/solana-accountsdb-sqs): A Geyser interface to write to SQS. By the Triton team.
 * [Kafka](https://github.com/Blockdaemon/solana-accountsdb-plugin-kafka): A Geyser plugin to publish to Kafka. By the Blockdaemon team.
 * [Bigtable](https://github.com/lijunwangs/solana-accountsdb-plugin-bigtable): WIP progress (non production ready) for Google Big Table. By Solana team.

## Geyser related

 * [Solana Postgres RPC server](https://github.com/lijunwangs/solana-postgres-rpc-server): A server to respond to RPC requests via Postgres data written by the Postgres plugin.
 * [gRPC connector](https://github.com/ckamm/solana-accountsdb-connector/tree/master/connector-mango): A connector that connects to gRPC plugin to parse data received.
