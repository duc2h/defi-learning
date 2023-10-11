I collect some my research about DEFI concepts.

### Smart contract (SC):
It is defined by collect of code. Nobody can control SC (in runtime), user can interact with SC via network (after SC deployed). When users execute a transaction that means users execute a function defined in SC. 

* Automic excution: Automatic run a demand (regularly defined by code) with no need for human participants.


Ref: https://ethereum.org/en/developers/docs/smart-contracts/

https://ethereum.org/en/smart-contracts/

How to Defi (page 21).


### Transaction:
It is the transaction between 2 addresses sender and receipt. The transaction is successful when the validators (blocks) have confirmed the transaction is successful.

Type of transaction:
1. Regular transactions: a transaction from one account to another.
2. Contract deployment transactions: a transaction without a 'to' address, where the data field is used for the contract code.
3. Execution of a contract: a transaction that interacts with a deployed smart contract. In this case, 'to' address is the smart contract address.

Transaction life cycle: https://ethereum.org/en/developers/docs/transactions/#transaction-lifecycle

Question: How many blocks in a specific transaction?

Example: https://etherscan.io/txs

Ref: https://ethereum.org/en/developers/docs/transactions/

### Protocol:

Ref: https://www.coinbase.com/learn/crypto-basics/what-is-a-protocol

### Gas:
The gas is the cost of the computation transaction. Each gwei is equal to one-billionth of an ETH (0.000000001 ETH or 10^-9 ETH).
The formula of gas: `The total gas you pay is divided into two components: the base fee and the priority fee (tip).`
The base fee is set by the protocol - you have to pay at least this amount for your transaction to be considered valid. The priority fee is a tip that you add to the base fee to make your transaction attractive to validators so that they choose it for inclusion in the next block.

For example, let's say Jordan has to pay Taylor 1 ETH. An ETH transfer requires 21,000 units of gas, and the base fee is 10 gwei. Jordan includes a tip of 2 gwei.

The total fee would now be equal to: `units of gas used * (base fee + priority fee)`

where the base fee is a value set by the protocol and the priority fee is a value set by the user as a tip to the validator. i.e. 21,000 * (10 + 2) = 252,000 gwei (0.000252 ETH).

When Jordan sends the money, 1.000252 ETH will be deducted from Jordan's account. Taylor will be credited 1.0000 ETH. The validator receives the tip of 0.000042 ETH. The base fee of 0.00021 ETH is burned.

Ref: https://ethereum.org/en/developers/docs/gas/#what-is-gas
### Fee:
The reward for validator when they validate a transaction. 

* From the gas example: the fee for validator is 0.000042 ETH (21,000 * 2 * 10^-9).

### Token:

### Stable coin:
There are two type of stablecoins. Centralize and decentralize stablecoins.

* Centralize stablecoins: Every USDT is supposedly backed by $1 in the issuer’s bank account. However, one major downside to USDT is that users need to trust that the USD reserves are fully collateralized and actually exist.

* Decentralized stablecoins: It is created in a decentralized manner via an overcollateralization method, operate fully on decentralized ledgers, are governed by decentralized autonomous organizations, and its reserves can be publicly audited by anyone. i.e DAI,...

### Dapps:

### On-chain:
On-chain transaction: Transactions run directly on the blockchain.

Ref: https://coinmarketcap.com/alexandria/glossary/on-chain

https://www.coindesk.com/learn/on-chain-vs-off-chain-transactions-whats-the-difference/

https://www.youtube.com/watch?v=QmIK6UjxoVc
### Off-chain:
Off-chain transaction: Transactions run outside of the blockchain. It can be confirmed in two ways:
1. The transaction can be done through a separate transfer agreed upon by both parties with a third party acting as a guarantor helping validate and verify the terms of the agreement.
2. The transaction can occur through (layer 2)[https://www.ledger.com/academy/layer-2-blockchains-explained] which is a separate blockchain built on top of the existing main one. Once all the terms and conditions of the transaction have been met and both parties have completed their transactions => the transaction is executed and recorded on the blockchain  

### Signature:

Ref: https://www.coinbase.com/cloud/discover/dev-foundations/digital-signatures
https://goethereumbook.org/signatures/
Create a signature:
 https://app.mycrypto.com/sign-message

### EIP-712 typed data:

Ref: https://eips.ethereum.org/EIPS/eip-712
https://blog.hook.xyz/validate-eip-712/
https://medium.com/mycrypto/the-magic-of-digital-signatures-on-ethereum-98fe184dc9c7
https://medium.com/metamask/eip712-is-coming-what-to-expect-and-how-to-use-it-bb92fd1a7a26

### ABI
As Ethereum uses EVM(Ethereum Virtual Machine) as a core component of the network, smart contract code written in high-level languages needs to be compiled into EVM bytecode to be run. EMV Bytecode is an executable code on EVM and Contract ABI is an interface to interact with EVM bytecode. For example, if you want to call a function in a smart contract with your JavaScript code, ABI plays a role as an intermediary between your JavaScript code and EVM bytecode to interact with each other. Below diagram shows the architecture of Contract ABI, EVM bytecode and outside components(dApp and network). The left side is a process of compiling and the right side is interacting.

Ref: https://docs.soliditylang.org/en/latest/abi-spec.html
https://blog.chain.link/what-are-abi-and-bytecode-in-solidity/
https://github.com/crytic/evm-opcodes
https://medium.com/@eiki1212/explaining-ethereum-contract-abi-evm-bytecode-6afa6e917c3b

### ECDSA:

### Keccak256:


### ERC20:

Ref: https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/IERC20.sol#L4

### Contract account:

Ref: https://ethereum.org/en/developers/docs/standards/tokens/erc-20/
https://ethereum.org/en/developers/docs/accounts/#contract-accounts

### Oracle: 

### Pool:


### Liquidity:

### Liquidity provider:

### DEX

Uniswapv2: https://ethereum.org/en/developers/tutorials/uniswap-v2-annotated-code/

### Impermanent loss:

### Solidity: 

Ref: https://docs.soliditylang.org/en/v0.4.24/contracts.html#events

### Reorg:
A blockchain reorg is caused when two blocks are published at the same time. Short one- and two-block reorgs happen often because of network latency, but when reorgs extend for longer than one or two blocks, they can lead to malicious attacks or even network failure.

Ref: https://cointelegraph.com/explained/what-is-chain-reorganization-in-blockchain-technology
https://www.alchemy.com/overviews/what-is-a-reorg


### Sybil attack:

A Sybil attack in this case is a person or organization that creates hundreds or thousands of wallets and airdrops to make big profits. The purpose of this is to create a link between the wallets, thereby fooling the anti-Sybil system that all the wallets belong to an individual or organization. 