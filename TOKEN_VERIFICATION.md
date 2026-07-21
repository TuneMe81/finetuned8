# Token Address Verification - Issue #18

## Contract Addresses

### Contract 1: Primary Token
`0x2f3b7f2bdecb2414c004051195dabe3b8a359a01`

### Contract 2: NEW AGE TIME Token
`0x1c157faf68cf513fc8f881669061a5cc0dace38c`

## Issue Details
- **Issue #**: 18
- **Title**: milestone
- **Status**: Open
- **Blockchains**: Ethereum & Base
- **Issue URL**: https://github.com/TuneMe81/finetuned8/issues/18

## Ownership Verification

### Method 1: Check Contract Owner via Etherscan
1. Go to Etherscan for your contract
2. Look for "Contract" section
3. Find "Owner Address" or similar field
4. Verify the address matches your wallet

### Method 2: Get Signature Hash for Ownership Proof
To sign and prove ownership:

```
Message to Sign: "I verify ownership of contract [ADDRESS]"
Signature Algorithm: EIP-191 (personal_sign)
```

**Steps:**
1. Use wallet (MetaMask, Ethers.js, Web3.py, etc.)
2. Sign the message with your private key
3. You'll receive a signature hash (0x...)
4. Share the signature + message for verification

### Method 3: Transaction History Verification
1. Check first deployment transaction on Etherscan
2. Verify deployer address matches your wallet
3. Note the transaction hash for documentation

### Method 4: Smart Contract Function Call
1. Call `owner()` function on the contract
2. Compare returned address with your wallet
3. Document the result

### Method 5: Proxy Contract Verification
1. Check if contract is a proxy (most modern contracts are)
2. Verify the implementation contract address
3. Check owner of both proxy and implementation
4. Document both ownership chains

## Verification Checklist

### Address Format Validation
- [x] Valid address format
- [x] Correct checksum (if applicable)
- [ ] Address exists on blockchain

### Contract 1 Verification (0x2f3b7f2bdecb2414c004051195dabe3b8a359a01)
**Ethereum:**
- [ ] Contract deployed on Ethereum mainnet
- [ ] Verify contract source code on Etherscan
- [ ] Check contract ABI
- [ ] Validate token standard (ERC-20/ERC-721/etc)
- [ ] Confirm owner address
- [ ] Obtain signature hash proof

**Base:**
- [ ] Contract deployed on Base network
- [ ] Verify contract source code on BaseScan
- [ ] Check contract ABI
- [ ] Validate token standard
- [ ] Confirm owner address

### Contract 2 Verification (0x1c157faf68cf513fc8f881669061a5cc0dace38c) - NEW AGE TIME
**Ethereum:**
- [ ] Contract deployed on Ethereum mainnet
- [ ] Verify contract source code on Etherscan
- [ ] Check contract ABI
- [ ] Validate token standard (ERC-20/ERC-721/etc)
- [ ] Confirm owner address
- [ ] Obtain signature hash proof

**Base:**
- [ ] Contract deployed on Base network
- [ ] Verify contract source code on BaseScan
- [ ] Check contract ABI
- [ ] Validate token standard
- [ ] Confirm owner address

### Ownership Verification
- [ ] Owner addresses identified for both contracts
- [ ] Signature hashes obtained (if needed)
- [ ] Ownership proof documented

### Token Properties
- [ ] Token name
- [ ] Token symbol
- [ ] Decimals
- [ ] Total supply
- [ ] Owner/Creator verification

### Security Audit
- [ ] Contract audit status
- [ ] Known vulnerabilities
- [ ] Holder distribution analysis
- [ ] Verify contracts on explorers

## Explorer Links

### Contract 1: 0x2f3b7f2bdecb2414c004051195dabe3b8a359a01

**Ethereum:**
- Contract Explorer: https://etherscan.io/address/0x2f3b7f2bdecb2414c004051195dabe3b8a359a01
- Token Tracker: https://etherscan.io/token/0x2f3b7f2bdecb2414c004051195dabe3b8a359a01

**Base:**
- Contract Explorer: https://basescan.org/address/0x2f3b7f2bdecb2414c004051195dabe3b8a359a01
- Token Tracker: https://basescan.org/token/0x2f3b7f2bdecb2414c004051195dabe3b8a359a01

### Contract 2: 0x1c157faf68cf513fc8f881669061a5cc0dace38c (NEW AGE TIME)

**Ethereum:**
- Contract Explorer: https://etherscan.io/address/0x1c157faf68cf513fc8f881669061a5cc0dace38c
- Token Tracker: https://etherscan.io/token/0x1c157faf68cf513fc8f881669061a5cc0dace38c

**Base:**
- Contract Explorer: https://basescan.org/address/0x1c157faf68cf513fc8f881669061a5cc0dace38c
- Token Tracker: https://basescan.org/token/0x1c157faf68cf513fc8f881669061a5cc0dace38c

## Signature Tools
- **MetaMask**: Built-in signing via web3
- **Ethers.js**: `signer.signMessage(message)`
- **Web3.py**: `w3.eth.account.sign_message()`
- **MyEtherWallet**: Manual message signing

## Next Steps
1. Verify both contracts exist on Ethereum and Base networks
2. Identify and document owner addresses for both
3. Obtain signature hashes for ownership proof
4. Retrieve and validate contract ABIs from explorers
5. Check token metadata and properties on both chains
6. Document all findings for issue #18
