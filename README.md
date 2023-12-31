# Simulate a simple investment platform
Final project of fintech course in NTHU, 2022 Fall.   

## Abstract
使用者只需輸入想投資的標的，回測開始及結束時間，就能透過平台內各種投資策略得到sharpe ratio(SR)跟總投報率，來驗證我們提供的是能夠賺錢的方法。

## Method 1
i. EMA指標  
ii. KD指標  
iii. RSI  
- 以下表格為3種不同指標的實驗結果，輸入的標的都是ABBV，回測開始時間為2022-01-01，結束時間為2022-12-01。

|     | sharpe ratio | 總投報率 |
|  ----  | ----  | ----  |
| EMA指標 | 0.855 | 22.58% |
| KD指標 | 0.917 | 24.16% |
| RSI  | 0.835 | 23.75% |

- 使用回測框架: https://kernc.github.io/backtesting.py/

## Results
首先我們將5種方法，總共12種投資策略結合在同一個程式當中，並且模擬投資人實際回測的狀況，投資人只需輸入欲投資的標的，
回測開始及結束時間，就能從12種策略中得到總投報率及夏普值最好的2種投資策略。  
實例：投資人原先的資金有10000元，選擇投資的標的為AAPL，回測開始時間2020-01-01結束時間2022-01-01，
最後我們投資平台選擇出最好的投報率策略為使用趨勢因子surfing-trend作為投資策略，回測總投報率為231.58%，
最好的夏普值策略為使用波段力道作為投資策略，回測夏普值為3.61。

## More details
Please goto report.pdf

## Teamwork
|     | 貢獻 | 
|  ----  | ----  | 
| 林政緯 | 程式內容統整、報告及投影片撰寫、投影片報告 |
| **施詠舜** | Method 1，運用EMA、KD、RSI 來設計3種投資策略 | 
| 鄒汯憲 | Method 2，運用使用5力中的波段力道、趨勢力道、趨勢因子來設計3種投資策略 |
| 林恩同 | Method 3，運用5力基本面分數、月均價、季均價、日漲幅設計4種投資策略 | 
| 朱育民 | Method 4，運用趨勢力道和EMA 來設計投資策略 |  
| 劉杰 | Method 5，運用機器學習(Decision Tree)來設計投資策略 | 


