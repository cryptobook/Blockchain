## Blockchain

A blockchain is a sequence of linked blocks. Each block contains the hash value of the previous block 
A blockchain can be used as distributed ledger which records transactions in an efficient and verifiable way. Transactions in a block can not be modified without changing all subsequent hash values in the distributed copies of the blockchain.

The hashes of transactions $T_1, T_2, T_3, T_4, \dots$ form the leaves of a binary tree called Merkle tree. The nodes further up are hashes of two children nodes and the Merkle tree root is the top hash value.

This works with any even number of transactions.  The root hash identifies all transactions. Individual transactions can be authenticated by the hash path from leave to the root. Suppose we want to check if the transaction $T_3$ is contained in the blockchain.  Then we only need to verify  the hash path 
$H(T_3), H_{34}, H_{12}, H_{root}$. This is very efficient even for trees with thousands of  transactions. 

Blockchains are used by many cryptocurrencies. The blockchain records the transactions of previously unspent cybercoins from one or more input addresses to one or more output addresses. Each new block contains a proof-of-work; by adapting the nonce value a miner has to find a hash value of the new block that is smaller than the network's difficulty target. This requires a very large number of hashing operations which consumes significant computing resources and thus a lot of energy. The miner is rewarded with new cryptocoins. The proof of works also protects the blockchain against manipulations and complicates forks. 

