# Legacy Farm Contracts

If you've forgotten about your old Elk LP tokens in an older farm that is not accessible on [https://app.elk.finance](https://app.elk.finance), you can feel free to follow this tutorial to withdraw your LP tokens, and claim your rewards and impermanent loss protection amount (if applicable). You can also follow a video guide [here](https://youtu.be/silWbW4FDR0). Please note that this method currently only works on desktop browser extensions of MetaMask. You can find a guide [here](https://docs.elk.finance/tutorials/desktop-metamask-on-mobile) on how to set up the desktop version of MetaMask on your mobile device.

1. Find the address of the farm you are stuck in from the [Elk.Finance Docs Addresses](https://docs.elk.finance/addresses) and make sure it is the correct farming round\

2. Go to the staking pool link, then click write contract. If the farm is not verified and you see no "write contract" option. Please skip to the section below.\

3. Click connect to Web 3 and "Approve" (you may have to do this twice on some explorers)\

4. Click "write" under "1. exit" and approve the transaction in MetaMask to withdraw your LP tokens, any remaining rewards, and impermanent loss coverage (if applicable)

### Is the contract unverified? Watch the video or follow the steps below it.

{% embed url="https://youtu.be/7HvDz8jEf5g" %}



1. Find contract address of farm you are stuck in at [https://docs.elk.finance/addresses](https://docs.elk.finance/addresses), and copy it to Notepad for later.\

2. Navigate to a contract address from the same round that is verified, even if it is on a different chain.\

3. Head to the verified contract, and copy the contract code, noting the solidity version.\

4. Go to [remix.ethereum.org](https://remix.ethereum.org), ensuring you are on the right chain that you need to withdraw from in MetaMask.\

5. Create a new .sol file in Remix (the little file button in the menu) and paste the contract in there.\

6. Go down to the compiler tab, select the version that you noted prior, and hit compile.\

7. Go down to the deploy and run transaction tab. Change the environment to injected web3, and approve to connect your MetaMask\

8. Change the gas to what the network expects in gwei, change the contract to Staking Rewards, and paste the contract address you noted earlier of the farm you are stuck in into "At Address" and then click "At Address"\

9. Uncollapse the "Stakingrewards At ADDRESS" menu that just appeared on the left of remix, click "exit" and confirm your transaction. If an additional gas menu pops up, like on AVAX, then fill both gwei fields with 225 and then confirm the transaction in Remix, and also in MetaMask (ensuring the gas isn't too expensive). This should pull your LP out. You're finished! Head to the pool at app.elk.finance and withdraw your liquidity.

If it failed, scroll down to the blue "balanceOf" field and past your MetaMask address in there, and click "balanceOf". If it shows a value of 0, then that means you actually do not have any LP in this particular farm. You can actually paste other farm addresses in the blue "At Address" field and repeat this step until you find the farm you are actually stuck in (it will return a non-zero value). Then simply follow the last two steps above.
