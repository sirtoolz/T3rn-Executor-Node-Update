# T3rn Executor Node Update

## Getting Started
- You can buy vps($7) from vpsdime.com and pay with crypto or with your credit card.
- Login to your vps with Termius and follow this guide
- Fund your wallet with Arb Sepolia, OP Sepolia, Blast Sepolia, Base Sepolia and BRN tokens.

## Executor Script

```
sudo apt update
sudo apt upgrade
```
```
sudo apt install build-essential
sudo apt install git -y
```
```
sudo apt install screen
screen -S t3rn
```
```
wget https://github.com/t3rn/executor-release/releases/download/v0.46.0/executor-linux-v0.46.0.tar.gz
```
```
tar -xvzf executor-linux-v0.46.0.tar.gz
```
```
cd executor/executor/bin
```
```
export NODE_ENV=testnet
export LOG_LEVEL=debug
export LOG_PRETTY=false
```
```
export EXECUTOR_PROCESS_ORDERS=true
export EXECUTOR_PROCESS_CLAIMS=true
```
```
export PRIVATE_KEY_LOCAL=REPLACE-WITH-YOU-PRIVATE-KEY
```
```
export ENABLED_NETWORKS='base-sepolia,optimism-sepolia,l1rn,blast-sepolia,arb-sepolia'

export EXECUTOR_PROCESS_PENDING_ORDERS_FROM_API=false
export EXECUTOR_PROCESS_ORDERS_API_ENABLED=false
export EXECUTOR_ENABLE_BATCH_BIDING=true
export EXECUTOR_PROCESS_BIDS_ENABLED=true
```
```
export RPC_ENDPOINTS_bssp='you rpc or public rpc'
export RPC_ENDPOINTS_opsp='you rpc or public rpc'
export API_ENDPOINTS_L1RN='https://brn.rpc.caldera.xyz/'
export RPC_ENDPOINTS_blast='https://sepolia.blast.io/'
export RPC_ENDPOINTS_arb='https://arbitrum-sepolia-rpc.publicnode.com/
```
```
./executor
```
```
```
## NOTE
Use CTRL+A+D to minimize the T3RN screen
Use Screen -r T3rn to go back to executor screen
