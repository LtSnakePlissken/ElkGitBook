---
description: Guides for setting up farms, including links to FaaS on BTTC Testnet
---

# FaaS: Farm-as-a-Service

See here for the audit of our FaaS contracts:

{% file src="../.gitbook/assets/BiPole FaaS Audit.pdf" %}
FaaS Audit by BiPole
{% endfile %}



Below you will find links to the BTTC Testnet FaaS contracts as well as a guide to test out our beta FaaS contracts on BTTC Testnet. This section will be updated for all chains as all FaaS features roll out. Testing the FaaS UI will be possible through the Farm page at [https://elkdex-beta.herokuapp.com/farms](https://elkdex-beta.herokuapp.com/farms). Please head to this and follow the prompts to test out farm creation/deposits.

#### Requirements:

* Native tokens for gas fee. Click [here](https://testfaucet.bt.io/#/) for a link to a faucet to obtain free testnet BTT
* FaaS fee (currently 100 ELK on testnet) in wallet. &#x20;
  * Add BTTC Testnet to Metamask and use the [faucet](https://testnet.bttcscan.com/address/0xedcf2f457f3ad2bb50b6dc5e70daf29c57b0c00c#writeContract).  Connect your wallet by clicking "Connect to Web3" and approve the BTTC Testnet to be added to Metamask if you have not previously added it. The [faucet](https://testnet.bttcscan.com/address/0xedcf2f457f3ad2bb50b6dc5e70daf29c57b0c00c#writeContract) will allow you to obtain ELK for testing.
* A liquidity pair (ELP tokens) consisting of 2 tokens made using the [pool page](https://elkdex-beta.herokuapp.com/add/BTT/0xeEeEEb57642040bE42185f49C52F7E9B38f8eeeE)

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

**PLEASE NOTE:** _<mark style="color:red;">Reflection Tokens (with transfer taxes etc.) are NOT supported by FaaS. Any use of FaaS with these tokens will result in unusual behaviours so AVOID using FaaS for these tokens!</mark>_

_\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*_

## FaaS Guide

1. Navigate to [https://elkdex-beta.herokuapp.com/farms](https://elkdex-beta.herokuapp.com/farms) and connect your wallet.
2. Click "Create Farm".

<figure><img src="../.gitbook/assets/image (42).png" alt="" width="377"><figcaption><p>Click "Create Farm"</p></figcaption></figure>

3.  Choose the two tokens for farm creation.

    <figure><img src="../.gitbook/assets/image (35).png" alt="" width="356"><figcaption><p>If you have not yet created a pool (ELP), clicking next here will direct you to create it</p></figcaption></figure>


4.  Select the token(s) you'd like to reward to farmers. Click "+ Add" to reward additional tokens.

    <figure><img src="../.gitbook/assets/image (46).png" alt="" width="349"><figcaption><p>"Farming Period" denotes how long the farm will remain active</p></figcaption></figure>


5.  Select the deposit/withdrawal fees that users will pay to enter the farm.

    <figure><img src="../.gitbook/assets/image (43).png" alt="" width="356"><figcaption><p>Toggle on a withdrawal fee if desired</p></figcaption></figure>


6.  Set withdrawal fees, if desired.

    <figure><img src="../.gitbook/assets/image (40).png" alt="" width="320"><figcaption><p>Withdrawal fees must have decreasing fees and increasing days. In the example below, users have a 1% fee of deposited ELP for withdrawal before 1 day, then a 0.5% fee for withdrawal before 2 days, and a 0% withdrawal fee after 3 days.</p></figcaption></figure>


7.  Choose a date to start the farm, or start it now.

    <figure><img src="../.gitbook/assets/image (36).png" alt="" width="356"><figcaption></figcaption></figure>


8.  Confirm your farm details and deploy.

    <figure><img src="../.gitbook/assets/image (45).png" alt="" width="361"><figcaption><p>Approve and deploy farm! Ensure you have 1000 ELK to pay the deployment fee</p></figcaption></figure>


9.  Add reward tokens to the farm by entering the amount of each and clicking "Fund". Approve this transaction. Click "Start Farm" and approve this transaction as well.

    <figure><img src="../.gitbook/assets/image (44).png" alt="" width="359"><figcaption></figcaption></figure>


10. &#x20;That's it! Your farm now appears under the "[My Farms](https://elkdex-beta.herokuapp.com/farms/my)" tab on the "Farms" page.

    <figure><img src="../.gitbook/assets/image (34).png" alt="" width="380"><figcaption><p>Users can find your farm under the "All Farms Page"</p></figcaption></figure>

## Adding BTT Testnet

BitTorrent Chain Testnet:&#x20;

Network URL: https://pre-rpc.bt.io/

Chain ID: 1029

Currency symbol: BTT

Block explorer URL: https://testnet.bttcscan.com/

## Links to Smart Contracts

**BTTC Mainnet:**

Oracle:[ 0x8D09759d54a17aa31987a68F24fAE2a4C41A3203](https://bttcscan.com/address/0x8D09759d54a17aa31987a68F24fAE2a4C41A3203#writeContract)

FarmFactoryHelper: [0x40d4014b60dd73c7087d39b895aad2a698578175 ](https://bttcscan.com/address/0x40d4014b60dd73c7087d39b895aad2a698578175#code)

FarmFactoryHelperPermissioned: [0x8369a8ece09312166096e59cdf7451ffa7899701 ](https://bttcscan.com/address/0x8369a8ece09312166096e59cdf7451ffa7899701#code)

FarmFactory: [0xe2e239fc02fa9bd61ec12eee9f117482544852e2](https://bttcscan.com/address/0xe2e239fc02fa9bd61ec12eee9f117482544852e2#code)

FarmManager: [0x2369A48c2E858ca08A201015375914d12D9b8524](https://testnet.bttcscan.com/address/0x2369A48c2E858ca08A201015375914d12D9b8524#writeContract)

SingleStakeFactory: [0x83053944b99c4f25557570b301106f2fcf5019a2](https://bttcscan.com/address/0x83053944b99c4f25557570b301106f2fcf5019a2#writeContract)

SingleStakeManager: [0x713E6616b70267FD5f71A09B16688658488F3448](https://bttcscan.com/address/0x713E6616b70267FD5f71A09B16688658488F3448#code)

#### BTTC Testnet:

ElkDex Factory: [0x46C4f54F87889Fbd93Df80d8AaBa500268F2DDa8](https://testnet.bttcscan.com/address/0x46C4f54F87889Fbd93Df80d8AaBa500268F2DDa8#code)

ElkDex Router: [0x4360358F5E7A09b4c7690e50EA7e4D498c6D0671](https://testnet.bttcscan.com/address/0x4360358f5e7a09b4c7690e50ea7e4d498c6d0671)

ELK Faucet for Testing: [0xfaB91F3ADFfc7dA30fa1e0D897051476Ee1ebd61](https://testnet.bttcscan.com/address/0xfab91f3adffc7da30fa1e0d897051476ee1ebd61#writeContract)

Backup Faucet: [0xeDCf2f457f3AD2bb50B6dc5e70dAf29c57b0c00C](https://testnet.bttcscan.com/address/0xedcf2f457f3ad2bb50b6dc5e70daf29c57b0c00c#writeContract)

ElkDex Oracle: [0x8D09759d54a17aa31987a68F24fAE2a4C41A3203](https://testnet.bttcscan.com/address/0x8D09759d54a17aa31987a68F24fAE2a4C41A3203#writeContract)

Elk Farm Factory: [0xe2E239Fc02Fa9Bd61eC12eEE9F117482544852E2](https://testnet.bttcscan.com/address/0xe2E239Fc02Fa9Bd61eC12eEE9F117482544852E2#writeContract)

Elk Farm Factory Helper: [0x40D4014b60DD73C7087D39B895Aad2A698578175](https://testnet.bttcscan.com/address/0x40D4014b60DD73C7087D39B895Aad2A698578175)

Elk Farm Factory Helper (Permissioned): [0x8369a8eCe09312166096e59cDf7451ffa7899701](https://testnet.bttcscan.com/address/0x8369a8eCe09312166096e59cDf7451ffa7899701)

Elk Farm Manager: [0x2369A48c2E858ca08A201015375914d12D9b8524](https://testnet.bttcscan.com/address/0x2369A48c2E858ca08A201015375914d12D9b8524#writeContract)

Elk Single Stake Factory: [0x83053944b99c4F25557570B301106f2FCF5019a2](https://testnet.bttcscan.com/address/0x83053944b99c4F25557570B301106f2FCF5019a2#writeContract)

Elk Single Stake Manager: [0x713E6616b70267FD5f71A09B16688658488F3448](https://testnet.bttcscan.com/address/0x713E6616b70267FD5f71A09B16688658488F3448#writeContract)

## Testing with the Block Explorer

## Instructions for Testing FaaS on BTTC Testnet

You can also find definitions of various contract functions below. The same instructions apply for testing with Mainnet version, just with no faucet.

### Deploying a Farm

**FaaS Deployment Requirements:**

1. FaaS fee in wallet (currently 100 ELK on testnet only, 1000 ELK fee applies to Mainnet farm creation). Use the [faucet](https://testnet.bttcscan.com/address/0xedcf2f457f3ad2bb50b6dc5e70daf29c57b0c00c#writeContract) to obtain ELK on BTTC Testnet
2. Native tokens for gas fee. Click [here](https://testfaucet.bt.io/#/) for a link to a faucet to obtain testnet BTT free
3. Create Elk Liquidity Pool (ELP) using Router Contract (if pair has not already been created) ([https://testnet.bttcscan.com/address/0x4360358F5E7A09b4c7690e50EA7e4D498c6D0671#writeContract](https://testnet.bttcscan.com/address/0x4360358F5E7A09b4c7690e50EA7e4D498c6D0671#writeContract))
   * Follow these steps to create a new LP token using the addLiquidity or addLiquidity ETH (to add a BTT pair) function:
   * Ensure that you have enough of the two tokens in your wallet to provide liquidity and that you are [connected to the BTTC Testnet](https://doc.bt.io/docs/wallet) and have enough BTT for gas.
   * Approve the ElkRouter contract to spend both tokens (not necessary for BTT, just other tokens).&#x20;
   * You can do this by calling the approve function on each token contract by looking it up on the [BTTC Testnet Explorer](https://testnet.bttcscan.com/) after connecting your wallet to the BTTC Testnet Explorer by clicking “connect to web3”, going to “contract”, then “write contract” and passing the ElkRouter contract address (0xc06348AEE3f3E92eE452816E0D3F25C919F6fB04) and the desired amount (in Wei) as arguments and hitting “write”.
   * Navigate to the testnet [Elk Router Contract](https://testnet.bttcscan.com/address/0x4360358F5E7A09b4c7690e50EA7e4D498c6D0671#writeContract) on the testnet explorer
   * Call the addLiquidity function on the ElkRouter contract with the following parameters:
   * tokenA: The contract address of the first token.
   * tokenB: The contract address of the second token.
   * addLiquidityETH (this parameter is only for the addLiquidityETH function): The desired amount of BTT you want to provide as liquidity
   * amountADesired (or amountTokenMin for addLiquidityETH function): The desired amount of tokens you want to provide as liquidity \*\*
   * amountBDesired: The desired amount of tokens you want to provide as liquidity \*\*
   * amountETHmin (this parameter is only for the addLiquidityETH function): The minimum amount of BTT you're willing to provide. This is a safety check against slippage. For testing, this amount can be set 1% lower than addLiquidityETH.
   * amountAMin: The minimum amount of tokens you're willing to provide. This is a safety check against slippage. For testing, this amount can be set 1% lower than amountADesired.\*\*
   * amountBMin: The minimum amount of ELK tokens you're willing to provide. This is a safety check against slippage. For testing, this amount can be set 1% lower than amountBDesired.\*\*
   * to: The address that will receive the LP tokens. This can be your own wallet address.
   * deadline: A Unix timestamp representing the time until the transaction is valid. It prevents the transaction from being executed after the specified time. You can calculate the current UNIX time here [https://www.epochconverter.com/](https://www.epochconverter.com/) and add 100 to the number (e.g., 1681601694 becomes 1681601794).
   * Click “write” under the function and approve it in your wallet.
   * After executing the addLiquidity function, the ElkRouter will create a new LP token for the pair, and you'll receive the LP tokens in the specified to address. The LP tokens represent your share of the liquidity pool
   * \*\*This parameter is expecting a token value in Wei, so use a tool such as [https://eth-converter.com/](https://eth-converter.com/) to add the correct amount of 0s using the “Ether” field if the token you are adding has 18 decimals like most tokens
4. Navigate to ElkFarmFactory on the BTTC Testnet Explorer

### Deploying a new farm with the ElkFarmFactory using createNewRewards function

The process is the same with createNewPermissonedRewards but this type of farm allows the deployer to specify which wallets are whitelisted to enter the farm. The same steps apply to the ElkSingleStakeFactory except the user must utilize the createNewSingleStake function, ignoring the functions that do not appear below.

1. Ensure the ELK token is approved to be spent by the ElkFarmFactory for the initial 1k ELK fee by navigating to the explorer contract of ELK (e.g., to approve the ELK on BTTC testnet the user would navigate [here](https://testnet.bttcscan.com/address/0xeEeEEb57642040bE42185f49C52F7E9B38f8eeeE#writeContract))
2. \_lpTokenAddress: Enter address of Elk LP token for farm that is present in your wallet (e.g., WBTT-ELK is 0xBc7290F14662b2242c0F7B3A5fddE33Db74DF6A6)
3. \_coverageTokenAddress: Enter address of coverage token for Impermanent Loss Protection (ILP)
   * Either of the two tokens in the farm LP
   * Enter 0x0000000000000000000000000000000000000000 if ILP is not desired
4. \_coverageAmount: Amount of coverage to be paid out (with required decimals)
   * 0 = ILP is not desired
   * Note: Ensure token decimal format is correct (check token in explorer)
5. \_coverageVestingDuration: Duration of coverage vesting period in seconds
   1. Must be equal to at least 3 days (259200) and no longer than the rewards duration
   2. 0 = ILP is not desired
6. \_rewardTokenAddresses: a list of reward token addresses
   * Format: \[0xeEeEEb57642040bE42185f49C52F7E9B38f8eeeE, 0xc7198437980c041c805A1EDcbA50c1Ce5db95118]
   * A maximum of 15 tokens are allowed to be rewarded. The gas fee for deployment increases as more tokens are rewarded.
7. \_rewardsDuration: Duration of rewards period in seconds
   * Enter the duration period in seconds (e.g., 1 month of rewards = 2629743)
8. \_depositFeeBps: Deposit fee basis points are the fees taken from the user when depositing LP into the farm
   * Denominated in basis points (e.g., 100 = 1%)
   * 0 = no deposit fees
9. \_withdrawalFeesBps: List of withdrawal fees.
   * Denominated in basis points (e.g., 100 basis points = 1% withdrawal fee)
   * Example: \[2000,1000,0]. This example is 20%, 10%, 0%.
   * If fees are not desired, enter any 3 values in descending order \[3,2,1] and set \_withdrawalFeeSchedule to \[1,2,3]
10. \_withdrawalFeeSchedule: List of time in seconds
    * A schedule to apply to \_withdrawalFeesBps
    * Example: \[604800,1209600,1814400] = 20% fee if withdrawal is within 7 days, 10% between 7-14 days, and 0% after 21 days. The code checks if the stake time is between the blocktime + the schedule seconds. This would make it 20% for 7 days, 10% for 14 days, and then 0% after that.  If one were to add 5% as the last fee amount, it would apply for 14-21 days and then be 0 after that.
    * If no fee is desired, set this to \[1,2,3]
11. Press Write
    * The transaction will output an event that contains the address of the new FarmingRewards contract. Check the logs tab of the transaction in the explorer, and look for the 3rd entry (i.e., labeled “2”)

### Managing farms using FarmManager

**Requirements:**

1. A FarmingRewards contract address (from createNewRewards function)
   * FarmManager manages FarmingRewards contracts
   * Any calls to FarmManager must be from the same wallet used to deploy the FarmingRewards contract
   * The functions available in FarmManager are any that would normally require ownership of the farming contract.
   * The stake/withdraw/getRewards functions that farm users interact with via the UI can be called directly from the FarmingRewards contract.
2. Before starting the farm from FarmManager, be aware:
   * Any reward/ILP tokens must be sent to the FarmingRewards contract.
   * Know that rate of emission is determined using the rewardsDuration and the amount of tokens provided to the \_rewards parameter.
   * The \_rewards parameter is a list of token amounts ordered by the provided rewardTokenAddresses. If tokens are added or removed, the order can be checked using the \_rewards parameter variable.
3. Start the farm in FarmManager using startEmission or startEmission with Coverage for farms with ILP.
   * farmAddress: Address of farm to start emissions for
   * \_rewards: Amount of each token to emit. Order is tied to \_tokenAddresses field when ElkFarmFactory was used to create the farm.
   * \_coverage: Maximum amount of total ILP coverage token to emit over the duration of the reward period
   * \_duration: Duration to reward all tokens and ILP for (in seconds)

**FarmManager Functions**

1. addRewardToken: Adds more tokens for rewards to ELP added to the farm
   * farmAddress: The contract address of the created farmingRewards
   * \_tokenAddress: The contract address of the farm’s reward token

Note: A reward token can be sent to the farm by sending it to the farmingRewards contract

1. multiClaim: Allows users to claim all rewards from multiple farms
   * \_farms: Input the addresses of all farms the wallet can claim rewards from (e.g., \[0x0000000000000000000000000000000000000000,0x0000000000000000000000000000000000000001,0x0000000000000000000000000000000000000002] would allow the user to claim all rewards from these 3 farms)
2. recoverERC20: Allows farm creator wallet to claim any tokens sent to the contract that were not awarded
   * farmAddress: Contract address of created FarmingRewards contract
   * \_tokenAddress: Contract address of token to claim
   * \_amount: Amount of token to claim
3. recoverFees: Allows farm creator to claim deposit/withdrawal fees from farm.
   * farmAddress: Address of farm to claim FaaS fee from
4. recoverLeftoverCoverage: Allows farm creator to collect unawarded coverage token(s) for ILP
   * farmAddress: Address of farm to recover unused ILP from
5. recoverLeftoverReward: Allows farm creator to collect excesses unawarded reward tokens from farm contract
   * farmAddress: Address of farm to recover excess reward tokens from
   * \_tokenAddress: Address of token to be recovered
6. renounceOwnership: Accessible only by Elk multi-sig wallet. Removes ownership of farmManager contract.
7. setFarmFactory: Accessible only by Elk multi-sig wallet. Sets the contract address of the FarmFactory contract.
   * factoryAddress: Address of farmFactory contract
8. setAddressPermission: For permissioned farms, allows farm creator to authorize/revoke authorization to any address so it can deposit into the farm.
   * \_walletAddress: Address to allow/disallow
   * \_permission: True or False (Allow or disallow)
   * \_permissionedFarmAddress: Address of farm to add/remove wallet from
9. startEmission: Starts the reward token emissions for a single farm without ILP
   * farmAddress: Address of farm to start emissions for
   * \_rewards: Amount of each token to emit. Order is tied to \_tokenAddresses field when ElkFarmFactory is used to create a farm
   * \_duration: Duration to reward all tokens for (in seconds)
10. startEmission With Coverage: Starts the reward token emissions for a single farm with ILP
    * farmAddress: Address of farm to start emissions for
    * \_rewards: Amount of each token to emit. Order is tied to \_tokenAddresses field when ElkFarmFactory was used to create the farm.
    * \_coverage: Maximum amount of total ILP coverage token to emit over the duration of the reward period
    * \_duration: Duration to reward all tokens and ILP for (in seconds)
11. stopEmission: Stops the farm from awarding tokens
    * farmAddress: Address of farm to stop rewards for
12. transferOwnership: Accessible only by Elk multi-sig wallet. Transfers ownership of FarmManager to a new wallet.
    * newOwner: Address of new owner wallet
