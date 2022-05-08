# Speedrun Ethernaut With Foundry :shipit:

OpenZeppelin's wargame, [Ethernaut](https://ethernaut.openzeppelin.com/) teaches practical smart contract security concepts through CTF like challenges. 

This repo contains walkthroughs and solutions to each level using only [Foundry](https://book.getfoundry.sh/index.html).

#### Foundry's toolchain consists of :
- **`Forge`** a cli tool for testing, building, and deploying smart contracts
 
- **`Cast`** a swiss army knife for interacting with Ethereum RPC nodes
 
## How To Use This Repo
### Config & Setup
This project uses [environment variables](https://www.geeksforgeeks.org/environment-variables-in-linux-unix/) to handle all config variables:
- `ETH_RPC_URL` this is **automatically** checked by forge and cast
- `PRIVATE_KEY` this has to be **manually** included when using forge or cast
- `LEVEL_ADDRESS` instance address

Environment variables can be set in the terminal as follows
```
export PRIVATE_KEY=<your-private-key-here> 
export ETH_RPC_URL=<your-rinkerby-node-url-here>
export LEVEL_ADDRESS=<your-instance-address-here>
```

### Level Solution Navigation

| Level Name       | Concepts Explored                            | Difficulty |
| -----------      | -----------                                  | :----:     |
| Fallback         | Fallback & receive functions                 | 1/10       |
| Fallout          | Misnaming functions                          | 2/10       |
| Coin Flip        | Predicting onchain randomness                | 3/10       |
| Telephone        | Msg.sender vs tx.origin                      | 1/10       |
| Token            | Overflow and underflows attacks              | 3/10       |
| Delegation       | DelegateCall                                 | 4/10       |
| Force            | SelfDestruct function                        | 5/10       |
| Vault            | Inspecting contract storage slots            | 3/10       |
| King             | Spoofing contract that expects EOA           | 6/10       |
| Re-entrancy      | Re-entrancy attacks                          | 6/10       |
| Elevator         | Malicious interfaces                         | 4/10       |
| Privacy          | Layout of state variables in storage         | 8/10       |
| Gatekeeper One   | Bytemasking and gasLeft function             | 5/10       |
| Gatekeeper Two   |                                              | 6/10       |
| Naught Coin      | Inheritance and transferFrom function        | 5/10       |
| Preservation     | DelegateCall                                 | 8/10       |
| Recovery         | Contract address creation                    | 6/10       |
| Magic Number     | Contract init and runtime opcodes            | 6/10       |
| Alien Codex      | Writing to any storage slot using overflows  | 7/10       |
| Denial           | Ddos gas draining attack                     | 5/10       |
| Shop             | Malicious view function interfaces           | 4/10       |
| Dex              | Manipulating oracle-less price data          | 3/10       |
| Dex Two          | Creating a malicious ERC20 token             | 4/10       |
| Puzzle Wallet    |                                              | 7/10       |
| Motorbike        |                                              | 6/10       |
| DoubleEntryPoint |                                              | 4/10       |
