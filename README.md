# 2024-Spring-HW2

Please complete the report problem below:

## Problem 1
Provide your profitable path, the amountIn, amountOut value for each swap, and your final reward (your tokenB balance).

![image](https://github.com/wisley63/Homework2/assets/113053224/72335582-6cee-49cd-83d0-e9e63c86b879)

## Problem 2
What is slippage in AMM, and how does Uniswap V2 address this issue? Please illustrate with a function as an example.

In Automated Market Making (AMM), slippage refers to the difference between the expected price of an asset and the actual price at which the trade is executed. It occurs because the execution of a trade on an AMM platform can cause the asset price to move due to changes in the supply and demand of the assets in the pool.

Uniswap V2 addresses the issue of slippage by introducing a feature called "Constant Product Market Maker" mechanism. It ensures that the product of the reserve amounts of two assets in a liquidity pool remains constant. This means that as one asset is bought, the supply of that asset decreases and the price increases, preventing large slippage.

![image](https://github.com/wisley63/Homework2/assets/113053224/41b2ef44-0f76-4019-b9e9-7e18b59ce2a5)

## Problem 3
Please examine the mint function in the UniswapV2Pair contract. Upon initial liquidity minting, a minimum liquidity is subtracted. What is the rationale behind this design?

The rationale behind subtracting a minimum liquidity upon initial liquidity minting in the UniswapV2Pair contract is to ensure that liquidity providers contribute a meaningful amount of liquidity to the liquidity pool.

By subtracting a minimum liquidity amount, Uniswap ensures that liquidity providers contribute a sufficient level of liquidity to the pool to support efficient trading. This helps prevent the liquidity pool from being fragmented into many small liquidity positions, which could lead to inefficiencies, increased slippage, and reduced trading depth.

Additionally, requiring a minimum liquidity contribution incentivizes liquidity providers to contribute substantial liquidity, enhancing the overall trading experience for users and attracting more traders to the platform.

## Problem 4
Investigate the minting function in the UniswapV2Pair contract. When depositing tokens (not for the first time), liquidity can only be obtained using a specific formula. What is the intention behind this?

The intention behind using a specific formula for obtaining liquidity when depositing tokens (not for the first time) in the UniswapV2Pair contract is to ensure that the liquidity added to the pool is balanced relative to the existing reserves.

When depositing tokens into the liquidity pool, the specific formula is used to calculate the amount of liquidity tokens (LP tokens) that the liquidity provider will receive in exchange for their deposited tokens. This formula takes into account the current reserves of the tokens in the pool and ensures that the liquidity added is proportional to the existing reserves, maintaining the balance of the pool.

The formula typically calculates the amount of LP tokens using the constant product formula, which is a fundamental principle of automated market maker (AMM) systems like Uniswap. The constant product formula ensures that the product of the reserves of the tokens in the pool remains constant before and after a trade, thereby maintaining a balanced and efficient trading environment.

By using a specific formula for obtaining liquidity, Uniswap ensures that liquidity providers are fairly compensated for their contributions to the liquidity pool while maintaining the integrity and efficiency of the decentralized exchange ecosystem.


## Problem 5
What is a sandwich attack, and how might it impact you when initiating a swap?

A sandwich attack is a type of market manipulation that can occur on decentralized exchanges (DEXs) like Uniswap. In a sandwich attack, an attacker exploits the predictable price movement caused by the execution of a large trade to their advantage.

When initiating a swap on a decentralized exchange like Uniswap, a sandwich attack can impact you by causing:
Slippage: You might receive fewer tokens or pay more than expected due to price manipulation by attackers.
Front-Running: Attackers may exploit price movements caused by large trades, leading to unfavorable execution prices for your swap.
Loss of Funds: In extreme cases, you could experience significant losses if attackers successfully manipulate prices against your trade.
