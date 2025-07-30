# @soulwallet/sdk

## 0.4.1

### Patch Changes

- b5e3328: Refactored getUserOpHash to compute the hash using an EIP-712 domain separator for improved standards compliance. Updated test values to match the new hashing logic and adjusted packUserOp encoding to include a type hash.

## 0.4.0

### Minor Changes

- 7836109: Removed several unused ABI files (EIP1271Wallet, ERC20Paymaster, HelloWorld, IOracle, TestOracle, TokenERC20) and added ABI_IEntryPoint_v08. Updated ABI_DefaultCallbackHandler, ABI_ElytroDefaultValidator, ABI_ElytroFactory, and ABI_ElytroInstence with new functions and events. Adjusted tests to remove references to deleted ABIs. Updated Elytro-wallet-contract submodule. These changes align the ABI definitions and tests with the latest contract interfaces and codebase requirements.

### Patch Changes

- Updated dependencies [7836109]
  - @soulwallet/abi@0.5.0

## 0.3.14

### Patch Changes

- Updated dependencies [d1428f5]
  - @soulwallet/abi@0.4.0

## 0.3.13

### Patch Changes

- a3ae446: SoulWallet instances add parameter `_config` that can skip on-chain detection

## 0.3.12

### Patch Changes

- 08a29c6: 1. Fixed an issue with **UserOpReceipt** in `/sdk` 2. Updated `/assets` 3. Updated `/decoder`

## 0.3.11

### Patch Changes

- 03f6c19: Fixed some bugs

## 0.3.10

### Patch Changes

- 5e7a3ff: Allowed stateOverride parameter in estimateUserOperationGas function.

## 0.3.9

### Patch Changes

- 444ba80: The original struct is not modified by the function estimateUserOperationGas()

## 0.3.8

### Patch Changes

- 1f8b295: Fixed some bugs

## 0.3.7

### Patch Changes

- 5946781: Updated ethers to v6.13.2
- Updated dependencies [5946781]
  - @soulwallet/result@0.2.1
  - @soulwallet/abi@0.3.4

## 0.3.6

### Patch Changes

- 37f7773: - @soulwallet/decoder@0.3.2

  - Updated offline bytes4 list

  - @soulwallet/assets@0.3.1
    - Updated offline token list
  - @soulwallet/abi@0.3.2
    - Added zkEmail ABI
  - @soulwallet/sdk@0.3.5
    - Added static function `initializeData`
  - @soulwallet/zkemail
    - Server side zkEmail

- Updated dependencies [37f7773]
  - @soulwallet/abi@0.3.3

## 0.3.5

### Patch Changes

- Updated dependencies [910f948]
  - @soulwallet/abi@0.3.2

## 0.3.4

### Patch Changes

- b080ac3: 1. Compatibility with [savings](https://github.com/SoulWallet/soul-wallet-contract/commit/09082c1837df7c8c2f026b2e38775201a3bbf3bf) branch. 2. Removed `IL1KeyStore` from @soulwallet/sdk, added `SocialRecovery`.
- Updated dependencies [b080ac3]
  - @soulwallet/abi@0.3.1

## 0.3.3

### Patch Changes

- 01a952f: New function export: 'async getSemiValidSignature(args...) `

## 0.3.2

### Patch Changes

- c4026ab: Fixed bugs

## 0.3.1

### Patch Changes

- b81f625: Some optimizations:

  1. Temporarily restrict batch requests to the bundler.
  2. Removed fixed parameters from the constructor of SoulWallet and added variable parameters.

## 0.3.0

### Minor Changes

- 32f4da1: EntryPoint v0.7.0 Compatible

### Patch Changes

- Updated dependencies [32f4da1]
  - @soulwallet/abi@0.3.0

## 0.2.0

### Minor Changes

- ba276ce: Updated to support the latest contract

### Patch Changes

- Updated dependencies [ba276ce]
  - @soulwallet/result@0.2.0
  - @soulwallet/abi@0.2.0

## 0.1.15

### Patch Changes

- fee433c: Updating Project License to Reflect Accurate Licensing
- Updated dependencies [fee433c]
  - @soulwallet/result@0.1.3
  - @soulwallet/abi@0.1.4

## 0.1.14

### Patch Changes

- 654d182: Remove the hacky implementation in estimateUserOperationGas::callGasLimit.

## 0.1.13

### Patch Changes

- 26ebf12: Remove guardianSafePeriodMin restriction

## 0.1.12

### Patch Changes

- 010e96d: - @soulwallet/keyvault

  - Updated ethers.js -> 6.8.1

  - @soulwallet/decoder

    - Updated bytes4 dictionary for contracts

  - @soulwallet/assets

    - Updated ERC20 database

      ```shell
      + Big Time
      + iExec RLC
      ```

  - @soulwallet/abi

    - Updated contract ABI

      - ```
        ABI_KeystoreProof.ts
        	lastestProofL1BlockNumber -> latestProofL1BlockNumber

        ABI_SoulWallet.ts
        	hash -> rawHash
        ```

  - @soulwallet/sdk

    - Supported RS256 signature algorithm

      ```js
      export interface RSAPublicKey {
        /**
         * Hex string of public exponent
         *
         * @type {string}
         * @memberof RSAPublicKey
         */
        e: string;

        /**
         * Hex string of public key
         *
         * @type {string}
         * @memberof RSAPublicKey
         */
        n: string;
      }
      ```

- Updated dependencies [010e96d]
  - @soulwallet/abi@0.1.3

## 0.1.11

### Patch Changes

- e66af6c: Added recoverWebAuthNPublicKey() function

## 0.1.10

### Patch Changes

- Fix bug

## 0.1.9

### Patch Changes

- add securityControlModuleDelay argument

## 0.1.8

### Patch Changes

- 1. Added a local implementation compatible with webauthn.
  2. Allowed the minimum value for guardianSafePeriod to be 60\*1 (1 minute).

## 0.1.7

### Patch Changes

- fixed rawowners encode bug

## 0.1.6

### Patch Changes

- 774b525: EIP1271 EIP712-signature supported

## 0.1.5

### Patch Changes

- 1592675: Fix a bug in P256Lib caused by reference type

## 0.1.4

### Patch Changes

- Added L1KeyStore.getKeyHash(string[]) function

## 0.1.3

### Patch Changes

- Allow caller to customize nonce

## 0.1.2

### Patch Changes

- passkey version merged into soulwallet@npmjs.com
- Updated dependencies
  - @soulwallet/result@0.1.2
  - @soulwallet/abi@0.1.2

## 0.1.1

### Patch Changes

- fe0c28b: Initial release of the package.
- Updated dependencies [fe0c28b]
  - @soulwallet/result@0.1.1
  - @soulwallet/abi@0.1.1
