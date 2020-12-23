# Bug test case

To reprise the bug of MoonBeam run:

```
$ npx hardhat run deploy/sample.js --network moonbasealpha
ProviderError: Method not found
    at HttpProvider.request (/home/porton/t/moonbeam-deploy-bug/node_modules/hardhat/src/internal/core/providers/http.ts:46:19)
    at LocalAccountsProvider.request (/home/porton/t/moonbeam-deploy-bug/node_modules/hardhat/src/internal/core/providers/accounts.ts:131:34)
    at GanacheGasMultiplierProvider._isGanache (/home/porton/t/moonbeam-deploy-bug/node_modules/hardhat/src/internal/core/providers/gas-providers.ts:175:30)
    at GanacheGasMultiplierProvider.request (/home/porton/t/moonbeam-deploy-bug/node_modules/hardhat/src/internal/core/providers/gas-providers.ts:164:23)
    at EthersProviderWrapper.send (/home/porton/t/moonbeam-deploy-bug/node_modules/@nomiclabs/hardhat-ethers/src/ethers-provider-wrapper.ts:13:20)
    at Object.getSigners (/home/porton/t/moonbeam-deploy-bug/node_modules/@nomiclabs/hardhat-ethers/src/helpers.ts:35:20)
    at getContractFactoryByAbiAndBytecode (/home/porton/t/moonbeam-deploy-bug/node_modules/@nomiclabs/hardhat-ethers/src/helpers.ts:250:21)
    at main (/home/porton/t/moonbeam-deploy-bug/deploy/sample.js:3:21)
```