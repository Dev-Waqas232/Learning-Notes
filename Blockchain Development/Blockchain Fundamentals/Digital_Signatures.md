# Digital Signatures

This topic shows how cryptography is used to secure messages as it is the integral part of any blockchain

## Symmetric Key Cryptography ( Private Key Cryptography )

- Same key on both sides ( Used for military usage )
- Message is encrypted and decrypted using the same key ( like moving one character right or left )

### Downside

- Both parties must have the same key beforehand so they can translate the information out of the code
- So if the receiver doesn't have your key, it would be impossible to decrypt the message

## Asymmetric Key Cryptography ( Public Key Cryptography )

- Split a key into two keys, one would be private and other one will be public
- The person having his own private key can only decrypt the message because he has the private key
- Public keys can be used to verify that the message is sent by the person who sign a message with his private key
- Public key can't decrypt the message, can only verify using the public key ( Authentications )

## Public Key Cryptography in Blockchain

- When you create a wallet, it generates one private key for you and one public key for whole blockchain
- User signs a transaction with its private and broadcast it to the blockchain
- Blockchain uses that public key to verify your identity
