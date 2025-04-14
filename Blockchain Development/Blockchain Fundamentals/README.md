# 🔗 Blockchain Fundamentals

## Purpose of Blockchain

- Network of computers agreen upon the same state of data
- Anyone should be able to participate in this process
- No one should be able to control this process
- Blockchain was invented to solve trust issues in transactions and to create a system that is neutral to any censorship or bribe

## Cryptographic Hash Functions

- Hash function takes input of any size and turns it into fixed sized output

### Properties

- Specific input always map to specific output
- Can't guess the output by observing the outputs for similar inputs
- The only way to figure the input out by viewing the output is, just keep guessing the input
- It must be fast
- No collision ( almost always have different outputs )

### Usage

- For different sizes of input, we can create a fixed size hash function which would save us the memory ( also known as commitment )
- This thing is super critical for blockchains and smart contracts as they just have to save that hash output only
- Cryptographic functions are also super important for first blockchain consensus mechanism i.e, Proof of Work
