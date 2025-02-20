# Nexus Testnet II Prover Node 

## Method 1. Web Browser
Contribute to Nexus zkVM Prover : https://app.nexus.xyz/

Connect Wallet, Email (use same if did testnet 1) and copy your prover_id

## Method 2. Linux Server
- For Old User Do this step first
```console
rm -rf .nexus
```

---
*Install Dependencies*
```console
sudo apt update && sudo apt upgrade -y
```
```console
sudo apt install -y protobuf-compiler
```
```console
sudo apt install curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev  -y
```
```console
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
- Click Enter to install default system settings
```console
source $HOME/.cargo/env
```
```console
export PATH="$HOME/.cargo/bin:$PATH"
```
```console
rustup target add riscv32i-unknown-none-elf
```
```console
sudo apt-get remove -y protobuf-compiler && wget https://github.com/protocolbuffers/protobuf/releases/download/v30.0-rc1/protoc-30.0-rc-1-linux-x86_64.zip && unzip protoc-30.0-rc-1-linux-x86_64.zip -d /usr/local/ && sudo chmod +x /usr/local/bin/protoc
```


*Open screen*
```console
sudo apt install screen
```
```console
screen -S nexus
```

*Run:*
```console
sudo curl https://cli.nexus.xyz/ | sh
```
- Enter prover id you copied from web browser

---
- Done !! Feel free to ask queries in telegram channel
- Telegram - https://t.me/colonyairdrops
- Youtube - https://www.youtube.com/@ColonyAirdrops
- Twitter - https://x.com/colony_airdrops
