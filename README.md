# Standart SUI fungible tokens

## Install 
### Rust
Use the following command to install Rust and Cargo on macOS or Linux:
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Use the following command to update Rust with `rustup`:
```
rustup update stable
```
### Additional prerequisites by operating system
Use the following command to update `apt-get`:
```
sudo apt-get update
```
Run the following command to install all prerequisite  at once:
```
sudo apt-get install curl git-all cmake gcc libssl-dev pkg-config libclang-dev libpq-dev build-essential
```
### Sui
#### Install Sui binaries from source
Run the following command to install Sui binaries from the `testnet` branch:
```
cargo install --locked --git https://github.com/MystenLabs/sui.git --branch testnet sui
```
To update to the latest stable version of Rust:
```
rustup update stable
```
#### Upgrade Sui binaries
If you previously installed the Sui binaries, you can update them to the most recent release with the same command you used to install them:
```
cargo install --locked --git https://github.com/MystenLabs/sui.git --branch devnet sui
```
## Fungible Tokens

* MANAGED: a token managed by a treasurer trusted for minting and burning. This is how (e.g.) a fiat-backed stablecoin or an in-game virtual currency would work.
* BASKET: a synthetic token backed by a basket of other assets. This how (e.g.) a [Special Drawing Rights (SDR)](https://www.imf.org/en/About/Factsheets/Sheets/2016/08/01/14/51/Special-Drawing-Right-SDR)-like asset would work.
* REGULATED_COIN: a coin managed by a central authority which can freeze accounts

Also, don't forget about [the cheat sheet](https://docs.sui.io/guides/developer/dev-cheat-sheet)
