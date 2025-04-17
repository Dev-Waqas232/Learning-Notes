# Proof of Work

## Common issues

- How do all nodes agree on the state of account balance
- Who add new blocks/transactions to a chain
- How everything interact with each other while there is no central actor

- **The Solution** -> Consensus Mechanism

## Consensus Mechanism

- Consensus -> Coming to a general agreement
- Blockchain Consensus -> At least 51% of nodes should agree over the current global state of the whole network

## Proof of Work ( Used by bitcoin )

- Can't double spend ( Send a coin to the blockchain and then send same coin at the same time, impossible in real world scenario but possible in digital world )
- The longest chain will be the one on which everyone else will agree ( like 51% benchmark )

## Mining ( The "Work" in Proof of Work )

- Process of creating a block of transactions to be added to blockchain
- Mners -> Continously attempts to extend the chain with new blocks
- Miners are in charge of extending a blockchain by adding blocks that contain **valid** transactions
- Miners will be asked for the proof of their work in order to add the block to the chain

## How Mining Works

Mining is done by automated software, human only setup and maintain the hardware part

- Miners provide a piece of data i.e, header of previous block and new transaction to add to the chain, and hash it
- If output is below difficulty target, it will be added to the chain

## How POW Works

- They have some sort of target difficulty
- If they want to add the new block, they have to find a POW lower than the difficulty level
- It is real hard and take very much resources to find such a output
- Miner who finds the target output first get rewarded with compensation

## Example Algorithm

Here's what the proof-of-work mining algorithm looks like:

- Take current block’s block header, add mempool transactions
- Append a nonce, starting at nonce = 0
- Hash data from #1 and #2
- Check hash versus target difficulty (provided by protocol)
- If hash < target, puzzle is solved! Get rewarded.
- Else, restart process from step #2, but increment nonce
