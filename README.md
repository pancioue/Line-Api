lone login
=============
登入line developers  
__keyword:"line developers"__    
[line developers](https://developers.line.biz/zh-hant/)
一個provider為一個提供者(例如以網站區分provider)，provider有 Provider ID 
provider底下有Channel，Roles (可以以Channel區分網站底下的專案)  
在Roles下點擊Invite by email可以邀請其他line好友加入此Provider，並成為admin  
如此便不會有被帳號綁死的情況

成功邀請了Providers之後，登入該帳號就可以看到底下的Channels，但仍無法編輯  
若要編輯Channel要再另外邀請Channel Role

Channel
----------
大部分的設定都在Channel底下，分四個部分

### basic settings
可以看到Channel ID 及 Channel secret
是之後接line login要傳的`client_id`跟`client_secret`

### Line Login
設定Callback URL

### Roles
新增admin人員
若該人員已經加入Provider，可以直接點擊Import from provider列出可以匯入的人員

> LIFF沒用到



line pay
===============
line pay登入頁: https://pay.line.me/portal/tw/auth/login
點擊"以商店ID登入"tag並登入

line pay 有自己的developers  
__keyword:"line pay developer"__  
[線上串接文件](https://pay.line.me/tw/developers/apis/onlineApis?locale=zh_TW)

帳號分為店家帳號及經銷商帳號
線上(web)走經銷商帳號模式，線下(api)走店家帳號模式

線上:
線上因為有return url必須開通白名單
登入__經銷商帳號__後，可以看到側邊欄

在此設定白名單

<img src="https://user-images.githubusercontent.com/24542187/116396281-c7a48080-a857-11eb-8e9e-108d205e292c.jpg" width="300">


line notify
==============
line notify: https://notify-bot.line.me/zh_TW/  
登入後進到個人頁面


![notify_personal](https://user-images.githubusercontent.com/24542187/116398373-4d293000-a85a-11eb-88db-347b1d09058e.jpg)




發行權杖要選擇推波的群組，群組內的人都可以收到
發行權杖後，記下token

[LINE Notify API Document](https://notify-bot.line.me/doc/en/)
有教學呼叫api (找到https://notify-api.line.me/api/notify)

呼叫成功就可以收到notify  
<img src="https://user-images.githubusercontent.com/24542187/116396381-e7d43f80-a857-11eb-9679-81221f45deae.jpg" width="300">
