** COINZ! **

Have you ever wondered how many BTC or ETH your crypto portolio would be worth
if you were to convert out of all your alt coins?  Introducing COINZ, a simple
executable bash script (with ruby under the hood) that will do just that!

Step 1: Edit the key.txt file and replace the current text with your coinmarketcap pro api key

Step 2: Edit the tokens.yml file and add your token holdings

```
  ---
  dash: 22
  litecoin: 44
  ethereum-classic: 503.12
  basic-attention-token: 12_345.6
  golem-network-tokens: 1000
  pivx: 500
```

Step 3: Run the coinz script

```
  > ./coinz
```

Step 3: Observe your holdings and notice how many BTC or ETH you could have if you were to sell all your alt coins:

```
****************************************************************************************************
DASH: 22 @ $342.698 is worth: $7,539.35 / 2.033 BTC / 26.531 ETH
LTC: 44 @ $48.2077 is worth: $2,121.13 / 0.572 BTC / 7.464 ETH
ETC: 503.12 @ $10.478 is worth: $5,271.72 / 1.422 BTC / 18.551 ETH
BAT: 12,345.6 @ $0.208093 is worth: $2,569.03 / 0.693 BTC / 9.048 ETH
GNT: 1,000 @ $0.250315 is worth: $250.31 / 0.067 BTC / 0.880 ETH
PIVX: 500 @ $2.86649 is worth: $1,433.24 / 0.386 BTC / 5.043 ETH
****************************************************************************************************
Total value of assets: $19,184.81 / 5.176 BTC / 67.519 ETH
****************************************************************************************************
```

Step 4: Smile and take comfort that you are a part of the financial revolution!

---

Additionally, you can pass in price overrides as arguments to see what your portfolio might look like with tokens at those prices.  For example:


```
  > ./coinz LTC=200 GNT=10.25

****************************************************************************************************
DASH: 22 @ $342.698 is worth: $7,539.35 / 2.030 BTC / 40.359 ETH
LTC: 44 @ $200.0 is worth: $8,800.0 / 2.370 BTC / 47.108 ETH
ETC: 503.12 @ $10.478 is worth: $5,271.69 / 1.419 BTC / 28.220 ETH
BAT: 12,345.6 @ $0.208093 is worth: $2,569.03 / 0.691 BTC / 13.752 ETH
GNT: 1,000 @ $10.25 is worth: $10,250.0 / 2.760 BTC / 54.870 ETH
PIVX: 500 @ $2.86649 is worth: $1,433.24 / 0.386 BTC / 7.672 ETH
****************************************************************************************************
Total value of assets: $35,863.32 / 9.658 BTC / 191.984 ETH
****************************************************************************************************
```

You can also add a currencies environment variable to specify which currencies to compare against:


```
  > ./coinz currencies=usd,bch,eos

****************************************************************************************************
DASH: 22 @ $342.69 is worth: $7,539.35 / 5.338 BCH / 1849.313 EOS
LTC: 44 @ $48.20 is worth: $2,121.13 / 1.502 BCH / 520.289 EOS
ETC: 503.12 @ $10.47 is worth: $5,271.69 / 3.733 BCH / 1293.082 EOS
BAT: 12345.6 @ $0.20 is worth: $2,569.03 / 1.819 BCH / 630.152 EOS
GNT: 1000 @ $0.25 is worth: $250.31 / 0.177 BCH / 61.399 EOS
PIVX: 500 @ $2.86 is worth: $1,433.24 / 1.014 BCH / 351.557 EOS
****************************************************************************************************
Total value of assets: $19,184.77 / 13.585 BCH / 4705.796 EOS
****************************************************************************************************
```

