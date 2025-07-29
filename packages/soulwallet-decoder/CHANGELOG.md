# @soulwallet/decoder

## 0.5.0

### Minor Changes

- 7836109: Removed several unused ABI files (EIP1271Wallet, ERC20Paymaster, HelloWorld, IOracle, TestOracle, TokenERC20) and added ABI_IEntryPoint_v08. Updated ABI_DefaultCallbackHandler, ABI_ElytroDefaultValidator, ABI_ElytroFactory, and ABI_ElytroInstence with new functions and events. Adjusted tests to remove references to deleted ABIs. Updated Elytro-wallet-contract submodule. These changes align the ABI definitions and tests with the latest contract interfaces and codebase requirements.

### Patch Changes

- Updated dependencies [7836109]
  - @soulwallet/assets@0.4.0
  - @soulwallet/abi@0.5.0

## 0.4.0

### Minor Changes

- d1428f5: 1. Updated the contract ABI. 2. The current project plan is deprecated. 3. Updated the assets package.

### Patch Changes

- Updated dependencies [d1428f5]
  - @soulwallet/abi@0.4.0
  - @soulwallet/assets@0.3.5

## 0.3.5

### Patch Changes

- 08a29c6: 1. Fixed an issue with **UserOpReceipt** in `/sdk` 2. Updated `/assets` 3. Updated `/decoder`
- Updated dependencies [08a29c6]
  - @soulwallet/assets@0.3.4

## 0.3.4

### Patch Changes

- 5946781: Updated ethers to v6.13.2
- Updated dependencies [5946781]
  - @soulwallet/assets@0.3.3
  - @soulwallet/result@0.2.1
  - @soulwallet/abi@0.3.4

## 0.3.3

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
  - @soulwallet/assets@0.3.2
  - @soulwallet/abi@0.3.3

## 0.3.2

### Patch Changes

- 910f948: Update to the latest contract version compatible.
- Updated dependencies [910f948]
  - @soulwallet/abi@0.3.2

## 0.3.1

### Patch Changes

- b080ac3: 1. Compatibility with [savings](https://github.com/SoulWallet/soul-wallet-contract/commit/09082c1837df7c8c2f026b2e38775201a3bbf3bf) branch. 2. Removed `IL1KeyStore` from @soulwallet/sdk, added `SocialRecovery`.
- Updated dependencies [b080ac3]
  - @soulwallet/assets@0.3.1
  - @soulwallet/abi@0.3.1

## 0.3.0

### Minor Changes

- 32f4da1: EntryPoint v0.7.0 Compatible

### Patch Changes

- Updated dependencies [32f4da1]
  - @soulwallet/assets@0.3.0
  - @soulwallet/abi@0.3.0

## 0.2.0

### Minor Changes

- ba276ce: Updated to support the latest contract

### Patch Changes

- Updated dependencies [ba276ce]
  - @soulwallet/assets@0.2.0
  - @soulwallet/result@0.2.0
  - @soulwallet/abi@0.2.0

## 0.1.5

### Patch Changes

- fee433c: Updating Project License to Reflect Accurate Licensing
- Updated dependencies [fee433c]
  - @soulwallet/assets@0.1.4
  - @soulwallet/result@0.1.3
  - @soulwallet/abi@0.1.4

## 0.1.4

### Patch Changes

- 97c253e: Updated bytes4 signature list

## 0.1.3

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
  - @soulwallet/assets@0.1.3
  - @soulwallet/abi@0.1.3

## 0.1.2

### Patch Changes

- passkey version merged into soulwallet@npmjs.com
- Updated dependencies
  - @soulwallet/assets@0.1.2
  - @soulwallet/result@0.1.2
  - @soulwallet/abi@0.1.2

## 0.1.1

### Patch Changes

- fe0c28b: Initial release of the package.
- Updated dependencies [fe0c28b]
  - @soulwallet/assets@0.1.1
  - @soulwallet/result@0.1.1
  - @soulwallet/abi@0.1.1
