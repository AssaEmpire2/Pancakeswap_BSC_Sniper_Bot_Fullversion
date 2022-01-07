# 🚀 Pancakeswap BSC Sniper Bot 🚀
![TradingTigers](https://camo.githubusercontent.com/903e37c7728f19549eb56fcf25babe248bc6dea2d50fea0292c497b17a70eed9/68747470733a2f2f646f63732e70616e63616b65737761702e66696e616e63652f7e2f66696c65732f76302f622f676974626f6f6b2d32383432372e61707073706f742e636f6d2f6f2f6173736574732532462d4d48524558374448636c6a625935496b6a674a2532462d4d6246535033324b7079584c756a62453646442532462d4d62465355486f7351696f455f68384f674462253246646f63732532306d61737468656164253230283231292e706e673f616c743d6d6564696126746f6b656e3d33346134346532302d313731662d343364372d396336322d613835633231333061373431)  
Web3 Pancakeswap Sniper && Take Profit/StopLose bot written in python3, Please note the license conditions!
### The second Binance Smart Chain sniper bot with Honeypot checker!  
![Sniper](Screenshot.png)  
# Infos
This Tool only buys/sells with/to BNB but use Multi Hops to get the best Output!
Attention, You pay **[0.1% Tax]** on your swap amount!

### Support Us&You by Buying [SavannahCat Token](https://bscscan.com/token/0x6989e34b435798f401d4ffc8987cdb8fa4d61766?a=0x0a4a569cfa700fc2a1d54974712716e537c169ff)  
![Sniper](https://camo.githubusercontent.com/903e37c7728f19549eb56fcf25babe248bc6dea2d50fea0292c497b17a70eed9/68747470733a2f2f646f63732e70616e63616b65737761702e66696e616e63652f7e2f66696c65732f76302f622f676974626f6f6b2d32383432372e61707073706f742e636f6d2f6f2f6173736574732532462d4d48524558374448636c6a625935496b6a674a2532462d4d6246535033324b7079584c756a62453646442532462d4d62465355486f7351696f455f68384f674462253246646f63732532306d61737468656164253230283231292e706e673f616c743d6d6564696126746f6b656e3d33346134346532302d313731662d343364372d396336322d613835633231333061373431)  

# Download
### If you are not familiar with Python please have a look at [Releases](https://github.com/Trading-Tiger/Pancakeswap_BSC_Sniper_Bot/releases), there you can download Windows executable.
### Setup your Address and secret key in Settings.json and Run main-GUI.exe.

# Install
**First of all, you need install Python3+**
Run on Android you need Install [Termux](https://termux.com/)  
```shell
termux: $ pkg install python git
Debian/Ubuntu: $ sudo apt install python3 git make gcc
Windows: Need to install Visual Studio BuildTools & Python3
```

### Setup your Address and secret key in Settings.json.

Clone Repo:  
```shell
git clone https://github.com/Trading-Tiger/Pancakeswap_BSC_Sniper_Bot
cd Pancakeswap_BSC_Sniper_Bot
```

Install Requirements:  
```python
python(3) -m pip install -r requirements.txt
```  

Start Sniper:  
```python
python(3) Sniper.py -t <TOKEN_ADDRESS> -a <AMOUNT> -tx <TXAMOUNT> -hp -wb <BLOCKS WAIT BEFORE BUY> -tp <TAKE PROFIT IN PERCENT> -sl <STOP LOSE IN PERCENT>
python(3) Sniper.py -t 0x34faa80fec0233e045ed4737cc152a71e490e2e3 -a 0.001 -tx 2 -hp  -wb 10 -tp 50
python(3) Sniper.py -t 0x34faa80fec0233e045ed4737cc152a71e490e2e3 --sellonly
python(3) Sniper.py -t 0x34faa80fec0233e045ed4737cc152a71e490e2e3 -a 0.001 --buyonly
python(3) Sniper.py -t 0x34faa80fec0233e045ed4737cc152a71e490e2e3 -tsl 10 -nb
```  

Here are all options with infos:  
```python3
*'-t' or '--token', Token for snipe e.g. "-t 0x34faa80fec0233e045ed4737cc152a71e490e2e3"
'-a' or '--amount', float, Amount in Bnb to snipe e.g. "-a 0.1"

'-tx' or '--txamount', how mutch tx you want to send? It split your BNB amount in e.g. "-tx 5"

'-wb' or '--awaitBlocks', default=0, Await Blocks before sending BUY Transaction. e.g. "-ab 50" 

'-hp' or '--honeypot', if you use this Flag, your token get checks if token is honypot before buy!

'-nb' or '--nobuy', No Buy, Skipp buy, if you want to use only TakeProfit/StopLoss/TrailingStopLoss
'-tp' or '--takeprofit', Percentage TakeProfit from your input BNB amount. e.g. "-tp 50" 
'-tsl'or '--trailingstoploss', 'Percentage Trailing-Stop-loss from your first Quote "-tsl 50"

'-so' or '--sellonly', Sell ALL your Tokens from given token address
'-bo' or '--buyonly', Buy Tokens with your given amount

* = require every time its runs!
```
## Trailing-Stop-Loss:
<img src="https://i.ytimg.com/vi/dZFb0-fwqOk/maxresdefault.jpg" height="400">
