# CryptoCurrency Category
This is a little api service for privoding the category of a cryptocurrency.

Similar to how each stock has its own industry classificaition, each cryptocurrency also has its own classification.  

Based on the 强者优势(I don't know which the exact english word should use. It means that the powerfull player in the market would lead the direction even sometimes they are wrong, because they are powerful). I would use the Binance's exsiting classifcation as a foundation, combined with third-party data from [CoinMarketCap](https://coinmarketcap.com), [CoinGecko](https://www.coingecko.com), and supplemented by manual analysis to give the classification.
## Usage
It's a FastAPI service deployed on cloud.  
```python
import requests
import json
payload = {"base": "BTC"}
url = "https://young-chamber-41337-67dbb5d1ef56.herokuapp.com/category"
cate = requests.post(url=rul, data=json.dumps(payload))
print(cate.json())   #{"base": "BTC","category": "POW"}
```
details can be found in [here](https://young-chamber-41337-67dbb5d1ef56.herokuapp.com/docs).
## log
##### 20230311 deploy demo
with only 378 coin which is on trading in Binance's spot market at this moment.  