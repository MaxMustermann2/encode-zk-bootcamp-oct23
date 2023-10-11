# Homework 3

In principle, how could you use Zokrates to verify that a certain address on Ethereum has say more than 1 ETH ?

Assuming that the requirement is for the address to be kept public, we will store the hashed version of the address in the verifier. The first step is for the verifier to check whether the hash of the (private) inputs matches the hashed value stored. This ensures that the address is not revealed to the verifier, and by extension, the Ethereum node.

Next, we need a proof for the balance. Luckily, Ethereum's state trie comes into the picture. The block header contains the Merkle root of the state trie, which in itself contains account proofs. Each account proof represents the Merkle proof of the account state `[nonce, balance, storageHash, codeHash]`. If the prover can generate an (encrypted) proof, that works upwards from the balance to the account root to the state root to the block hash, the verifier should be able to compare the block hash submitted in the proof to the actual block hash and validate everything accordingly.

- Account balance
- `[nonce, balance, storageHash, codeHash]`
- `accountStateRoot`
- `storageRoot`
- `blockHash`, when combined with other roots in the block
