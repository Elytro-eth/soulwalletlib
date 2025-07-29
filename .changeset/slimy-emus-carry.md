---
"@soulwallet/decoder": minor
"@soulwallet/assets": minor
"@soulwallet/abi": minor
"@soulwallet/sdk": minor
---

Removed several unused ABI files (EIP1271Wallet, ERC20Paymaster, HelloWorld, IOracle, TestOracle, TokenERC20) and added ABI_IEntryPoint_v08. Updated ABI_DefaultCallbackHandler, ABI_ElytroDefaultValidator, ABI_ElytroFactory, and ABI_ElytroInstence with new functions and events. Adjusted tests to remove references to deleted ABIs. Updated Elytro-wallet-contract submodule. These changes align the ABI definitions and tests with the latest contract interfaces and codebase requirements.
