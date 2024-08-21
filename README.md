# teleport
this is docker project for mpc nodes for teleport bridge backend
## Features
Lux Teleport has the following features:

1. Decentralized oracle operations using MPC
2. Decentralized permissioning using MPC
3. Zero knowledge transactions, signers don't know details about assets being teleported to and from supported chains.

## Installation
Clone the repository on all signers.

```
git clone https://github.com/luxfi/mpc_nodes_docker
```

Install docker on your computer.

Run project.

You need to generate mpc key shares keys1.store, keys2.store, keys3.store before starting this project.

## To generate key shares, please visit: 
https://github.com/luxfi/multi-party-ecdsa

copy keys1.store file to mpc_node_0/multiparty_ecdsa/keys.store
copy keys2.store file to mpc_node_0/multiparty_ecdsa/keys.store
copy keys3.store file to mpc_node_0/multiparty_ecdsa/keys.store

```
docker compose up -d
```

Stop process

```
docker compose down
```