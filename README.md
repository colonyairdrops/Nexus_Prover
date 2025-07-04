# Nexus Testnet III Prover Node 

## Method 1. Web Browser
Contribute to Nexus zkVM Prover : https://app.nexus.xyz/

Connect Wallet, Email (use same if did testnet 1 & 2)

## Method 2. Linux Server
- For Old User Do this step first
```
rm -rf .nexus
```

---
*Install Dependencies*
```
sudo apt update && sudo apt upgrade -y
```
```
sudo apt install -y protobuf-compiler
```
```
sudo apt install curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev  -y
```
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
- Click Enter to install default system settings
```
source $HOME/.cargo/env
```
```
export PATH="$HOME/.cargo/bin:$PATH"
```
```
rustup target add riscv32i-unknown-none-elf
```
```
sudo apt-get remove -y protobuf-compiler && wget https://github.com/protocolbuffers/protobuf/releases/download/v30.0-rc1/protoc-30.0-rc-1-linux-x86_64.zip && unzip protoc-30.0-rc-1-linux-x86_64.zip -d /usr/local/ && sudo chmod +x /usr/local/bin/protoc
```


*Open screen*
```
sudo apt install screen
```
```
screen -S nexus
```

*Run*
```
sudo curl https://cli.nexus.xyz/ | sh
```
- Run with an existing node ID
```
source ~/.bashrc

nexus-network start --node-id your-node-id
```
- Replace `your-node-id` with the node_id from nexus dashboard or generate from CLI

*Get Node ID*

**1. Via Web**
- To get your node id visit [dashboard](https://app.nexus.xyz)
- Add Node --> Add CLI Node --> Copy your Node Id and use it in above step

**2. Via CLI**
- Register Wallet Address
```
nexus-network register-user --wallet-address your-wallet-address
```
- Replace `your-wallet-address` which you are using on Nexus Dashboard
```
nexus-network register-node
```
```
nexus-network start
```
- The `register-user` and `register-node` commands will save your credentials to `~/.nexus/credentials.json`

- To clear credentials, run:
```
nexus-network logout
```

*Accessing Screen Session*
- Use `CTRL A D` to detach from screen
- Use `screen -r nexus` to attach screen

---

*Update your Node*
```
screen -r nexus
```
- Type Q to quit the prover & type `clear` to clear the screen
```
sudo curl https://cli.nexus.xyz/ | sh
```
```
source ~/.bashrc
```
- Now Register your Node again using any of the above method

---
- Done !! Feel free to ask queries in telegram channel
- Telegram - https://t.me/colonyairdrops
- Youtube - https://www.youtube.com/@ColonyAirdrops
- Twitter - https://x.com/colony_airdrops
