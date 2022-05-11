## :satellite: Basic Smart Contract on NEAR 

An MVP (minimum viable product) for the most basic Rust smart contract you can possibly develop on NEAR Protocol. I recommedn you use this contract for reference and testing.

---

#### Execute Smart Contract :wrench: :gear:
These are the steps to execute a smart contract on NEAR:
* compile
* deploy
* interact

Run the following commands from terminal (from the root folder):
```bash
near login                                                               
near state accountname.testnet

export PATH="$HOME/.cargo/bin:$PATH"                                         
./build.sh                                                                   
near deploy accountname.testnet --wasmFile res/basic_crossword.wasm        
near view accountname.testnet get_puzzle_number
near call accountname.testnet set_solution '{"solution": "supercalifragilistichespiralidoso"}' --accountId accountname.testnet
near call accountname.testnet guess_solution '{"solution": "mysolutionguess"}' --accountId accountname.testnet
```
