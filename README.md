# solana-accountsdb-zoo

The solana accountsdb interface is a handy way to access both block and (in 1.9) transactions as they are processed by the validator.

This is a list of various accountsdb plugins available. Feel free to send a PR with your own.

For more info about the accountsdb interface: https://docs.solana.com/developing/plugins/accountsdb_plugin

## Plugins

 * [Postgres](https://github.com/solana-labs/solana-accountsdb-plugin-postgres): The OG plugin by the developers of the accountsdb interface in Solana team, supports inserting into postgres.
 * [gRPC](https://github.com/ckamm/solana-accountsdb-connector): A generic gRPC interface along with a sample plugin for writing the gRPC stream to postgres. By the Mango team.
 * [RabbitMQ](https://github.com/holaplex/solana-indexer/tree/dev/crates/accountsdb-rabbitmq): A RabbitMQ writer by the Holaplex team.
 * [SQS](https://github.com/rpcpool/solana-accountsdb-sqs): An accounts DB interface to write to SQS. By the Triton team.
 * [Kafka](https://github.com/Blockdaemon/solana-accountsdb-plugin-kafka): A Solana plugin to publish to Kafka. By the Blockdaemon team.

## AccountsDB related

 * [Solana Postgres RPC server](https://github.com/lijunwangs/solana-postgres-rpc-server): A server to respond to RPC requests via Postgres data written by the Postgres plugin.
 * [gRPC connector](https://github.com/ckamm/solana-accountsdb-connector/tree/master/connector-mango): A connector that connects to gRPC plugin to parse data received.
