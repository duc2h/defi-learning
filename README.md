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

From the gas example: the fee for validator is 0.000042 ETH (21,000 * 2 * 10^-9).

### Token:

### Stable coin:
There are two type of stablecoins. Centralize and decentralize stablecoins.

* Centralize stablecoins: Every USDT is supposedly backed by $1 in the issuer’s bank account. However, one major downside to USDT is that users need to trust that the USD reserves are fully collateralized and actually exist.

* Decentralized stablecoins: It is created in a decentralized manner via an overcollateralization method, operate fully on decentralized ledgers, are governed by decentralized autonomous organizations, and its reserves can be publicly audited by anyone. i.e DAI,...

### Dapps:

### On-chain:

Ref: https://coinmarketcap.com/alexandria/glossary/on-chain

### Off-chain:

### Oracle: 

### Pool:


### Liquidity:

### Liquidity provider:

### DEX


### Impermanent loss:

