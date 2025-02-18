# Nexus_Prover by @ColonyAirdrops

- Video: [Youtube](https://youtu.be/j2kyQtwtmjw)

## Method 1. Web Browser
Contribute to Nexus zkVM Prover : https://app.nexus.xyz/


## Method 2. Linux Server
**1. Install Dependecies**
```console
sudo apt update && sudo apt upgrade -y
```
**2. Install packages**
```console
sudo apt install curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev  -y
```
**3. Install Rust**
```console
sudo curl https://sh.rustup.rs -sSf | sh
```
**4. Add Rust to path**
```console
source $HOME/.cargo/env
export PATH="$HOME/.cargo/bin:$PATH"
```
```console
rustup update

rustc --version
```
```console
sudo apt install -y protobuf-compiler
```

**5. Run Prover**

*Open screen*
```console
screen -S nexus
```
*Run:*
```console
sudo curl https://cli.nexus.xyz/ | sh
```
- Enter prover id (watch youtube video to know how to get)

To minimize screen: `CTRL+A+D`

To retun screen: `screen -r nexus`

To run the prover again if faced any issues
```console
sudo curl https://cli.nexus.xyz/install.sh | sh
```

**3. Save Prover ID file**

You'll get a `prover-id` file in `/root/.nexus/` representing your unique contribution ID to Prover Node

![Screenshot_3](https://github.com/user-attachments/assets/5362c2b7-f116-4086-aeec-44fc7b425d05)


---
- Done !! Feel free to ask queries in telegram channel
- Telegram - https://t.me/colonyairdrops
- Youtube - https://www.youtube.com/@ColonyAirdrops
