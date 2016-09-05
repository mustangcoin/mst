xxxxxxxxxxxxxxxxxx
MustangCoin Specs:
------------------

nTargetSpacing = 1 * 60; // 60 seconds
nStakeMinAge = 24 * 60 * 60; // 24 hours
nStakeMaxAge = 30 * 24 * 60 * 60;           // 30 days
nModifierInterval = 10 * 60; // time to elapse before new modifier is computed
nCoinbaseMaturity = 40;
DAILY_BLOCKCOUNT =  1440;
MAX_BLOCK_SIZE = 2000000;
MIN_TX_FEE = 100000;
MAX_MONEY = 3000000 * COIN;
COIN_YEAR_REWARD = 12 * CENT; // 12% per year
MAX_MINT_PROOF_OF_STAKE = 0.12 * COIN;	// 12%


nSubsidy = nCoinAge * nRewardCoinYear / 365 / COIN;

nHeight+1 >= 0 && pindexBest->nHeight+1 <= 100)
nSubsidy = 0 * COIN;

nHeight+1 >= 101 && pindexBest->nHeight+1 <= 721)
nSubsidy = 333 * COIN;

nHeight+1 >= 722 && pindexBest->nHeight+1 <= 1440)
nSubsidy = 133 * COIN;

nHeight+1 >= 1441 && pindexBest->nHeight+1 <= 17280)
nSubsidy = 23 * COIN;

xxxxxxxxxxxxxxxxxxxxxxxxx
Sample mustang.conf file:
-------------------------

rpcuser=UserName
rpcpassword=YourSaltishPassworld 

rpcport=10193
port=10194

daemon=1
server=1
listen=1
rpcallowip=127.0.0.1


xxxxxxxxxxxxxxxxxxxxxxxxxxxx
