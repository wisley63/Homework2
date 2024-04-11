# 2024-Spring-HW2

Please complete the report problem below:

## Problem 1
Provide your profitable path, the amountIn, amountOut value for each swap, and your final reward (your tokenB balance).

Path: tokenB->tokenA->tokenE->tokenD->tokenC->tokenB

amount_in: 5.0, amount_out: 5.655321988655322
amount_in: 5.0, amount_out: 0.4865194583384165
amount_in: 5.0, amount_out: 1.6630525437864887
amount_in: 5.0, amount_out: 0.49874937468734365
amount_in: 5.655321988655322, amount_out: 2.372138936383089
amount_in: 5.655321988655322, amount_out: 2.4587813170979333
amount_in: 5.655321988655322, amount_out: 1.0583153138066885
amount_in: 0.4865194583384165, amount_out: 0.7128411757430962
amount_in: 0.4865194583384165, amount_out: 0.1909367676711635
amount_in: 0.4865194583384165, amount_out: 0.3700960449182321
amount_in: 1.6630525437864887, amount_out: 2.333533766053072
amount_in: 1.6630525437864887, amount_out: 3.6419439695291005
amount_in: 1.6630525437864887, amount_out: 0.6722816510514321
amount_in: 0.49874937468734365, amount_out: 1.8995515428188292
amount_in: 0.49874937468734365, amount_out: 0.5851927901368708
amount_in: 0.49874937468734365, amount_out: 1.1701334040063442
amount_in: 2.372138936383089, amount_out: 0.8768809049251629
amount_in: 2.372138936383089, amount_out: 1.5301371369636168
amount_in: 2.4587813170979333, amount_out: 5.0889272933015155
amount_in: 2.4587813170979333, amount_out: 0.9813249894861109
amount_in: 1.0583153138066885, amount_out: 1.1652391072917359
amount_in: 1.0583153138066885, amount_out: 2.429786260142227
amount_in: 0.7128411757430962, amount_out: 0.4071316230430122
amount_in: 0.7128411757430962, amount_out: 0.16367564504950055
amount_in: 0.1909367676711635, amount_out: 0.3107014448794441
amount_in: 0.1909367676711635, amount_out: 0.07906745567404347
amount_in: 0.3700960449182321, amount_out: 1.4432336466273696
amount_in: 0.3700960449182321, amount_out: 0.8726854758507169
amount_in: 2.333533766053072, amount_out: 1.2220531740659872
amount_in: 2.333533766053072, amount_out: 0.4986881565988928
amount_in: 3.6419439695291005, amount_out: 3.7570436807443435
amount_in: 3.6419439695291005, amount_out: 2.131032679121273
amount_in: 0.6722816510514321, amount_out: 2.4823463117499904
amount_in: 0.6722816510514321, amount_out: 0.7730615166757577
amount_in: 1.8995515428188292, amount_out: 1.028162049954426
amount_in: 1.8995515428188292, amount_out: 1.0089276914225063
amount_in: 0.5851927901368708, amount_out: 0.846292934221594
amount_in: 0.5851927901368708, amount_out: 0.22892281507534115
amount_in: 1.1701334040063442, amount_out: 1.721254447065056
amount_in: 1.1701334040063442, amount_out: 2.65813717790385
amount_in: 0.8768809049251629, amount_out: 0.35903943721878817
amount_in: 1.5301371369636168, amount_out: 3.450741448619708
amount_in: 5.0889272933015155, amount_out: 2.692729085985291
amount_in: 0.9813249894861109, amount_out: 1.0897076131383296
amount_in: 1.1652391072917359, amount_out: 0.44737293755283086
amount_in: 2.429786260142227, amount_out: 5.038996197252911
amount_in: 0.4071316230430122, amount_out: 0.16799276206608788
amount_in: 0.16367564504950055, amount_out: 0.3891032568195987
amount_in: 0.3107014448794441, amount_out: 0.07268247149804351
amount_in: 0.07906745567404347, amount_out: 0.32594814886154755
amount_in: 1.4432336466273696, amount_out: 0.7877736589965701
amount_in: 0.8726854758507169, amount_out: 1.3222818788111388
amount_in: 1.2220531740659872, amount_out: 0.8688500498078684
amount_in: 0.4986881565988928, amount_out: 0.5851251645701201
amount_in: 3.7570436807443435, amount_out: 0.7568510019597675
amount_in: 2.131032679121273, amount_out: 6.262412392231384
amount_in: 2.4823463117499904, amount_out: 1.2856715704476172
amount_in: 0.7730615166757577, amount_out: 1.091036774998018
amount_in: 1.028162049954426, amount_out: 0.3964834814790486
amount_in: 1.0089276914225063, amount_out: 2.3202565868449074
amount_in: 0.846292934221594, amount_out: 0.47929212181712155
amount_in: 0.22892281507534115, amount_out: 0.3709853846555979
amount_in: 1.721254447065056, amount_out: 0.9446798615114286
amount_in: 2.65813717790385, amount_out: 3.020859972607159

tokenB balance=20.042339589188174

## Problem 2
What is slippage in AMM, and how does Uniswap V2 address this issue? Please illustrate with a function as an example.

Slippage refers to the difference between the expected price of a trade and the actual price at which the trade is executed. In automated market maker (AMM) systems like Uniswap, slippage occurs because the price of a token changes with every trade due to the constant rebalancing of liquidity pools.
Uniswap V2 addresses the slippage issue by introducing a mechanism called "virtual balances and reserves." This mechanism allows traders to estimate the amount of slippage before executing a trade by considering the current liquidity in the pool.

## Problem 3
Please examine the mint function in the UniswapV2Pair contract. Upon initial liquidity minting, a minimum liquidity is subtracted. What is the rationale behind this design?

> Solution

## Problem 4
Investigate the minting function in the UniswapV2Pair contract. When depositing tokens (not for the first time), liquidity can only be obtained using a specific formula. What is the intention behind this?

> Solution

## Problem 5
What is a sandwich attack, and how might it impact you when initiating a swap?

> Solution

