# oose_0324082
資管系3B 0324082  陳毓廷 (組長)：上傳管理github、想法討論、製作APP。

資管系3B 0324038  黃珮禎：繪製圖表、想法討論、製作APP。

資管系3A 0324089  鄭婷瑀：想法討論、製作APP。

#_專題名稱：樓E幢_
###功能：

1.用戶登入：入住房東就給房客一組專用的帳密；房東也有一組專用的帳戶。

2.水電費：讓房客即時上網知道自己當月水電費，房東無須另外口頭或寄信通知。

3.設備維修：直接利用手機就可以讓房東知道維修項目。

4.門禁管理：使用手機NFC功能無需使用鑰匙以及感應卡就可進入大樓以及自己房間。

5.最新公告：房東以及房客可以即時上傳最新大樓的情況。例如：大樓電梯的損壞、或是臨時停電等。


###圖形介面：

####房東介面：

![image](https://cloud.githubusercontent.com/assets/22367717/19625894/7dfc02a0-9957-11e6-94e2-5463fb73bf10.jpg)

####房客介面：

![image](https://cloud.githubusercontent.com/assets/22367717/19625892/7dfa3128-9957-11e6-9ff9-d1b598418604.jpg)

###use case圖：

![image](https://cloud.githubusercontent.com/assets/22367717/21607675/b58efb04-d1f2-11e6-9b11-9e566a1525c4.png)

###系統活動圖：

![image](https://cloud.githubusercontent.com/assets/22367717/21607674/b5678d44-d1f2-11e6-937f-04c59dff22de.png)

###use case條件式描述：

####使用者個案名稱:房東登入

行為者：房東

目標：使房東能以app管理其他個案。

前提：房東須以房東身分登入系統。

－系列事件：

正常程序－

1.房東透過app進入系統登入帳號密碼。

2.系統驗證帳號密碼。

3.系統驗證房東登入成功。

例外狀況－

系統驗證不成功，房東登入失敗。


####使用者個案名稱：門禁管理

行為者：房東

目標：使房東能以帳密開啟房客進入大樓以及房間。

前提：房東要取得房客帳號密碼。

結束狀態：讓房客進入後，清除資料，回至首頁。

－系列事件：

正常程序－

1.房東透過app進入系統登入成功。

2.房東輸入房客帳密。

3.使房客進入大樓及租屋處。

例外狀況－

房客無忘記攜帶手機。

房東無法取得房客帳密。


####使用者個案名稱：水電費管理

行為者：房東

目標：使房東利用app給予每位房客當月水電費。

前提：房東已經計算好房客當月水電費。

結束狀態：輸入房號、當月月份和水電費，回至首頁。

－系列事件：

正常程序－

1.房東透過app進入系統登入成功。

2.房東輸入每位房客當月水電費。

例外狀況－

尚未收到當月水電費帳單，無法計算。


####使用者個案名稱：設備維修管理

行為者：房東

目標：使房客能以app通知房東需要維修設備。

前提：房客有提交維修事項。

結束狀態：房東已回復完成，並回至首頁。

－系列事件：

正常程序－

1.房東透過app進入系統登入成功。

2.回復房客維修日，及當日維修事項。

例外狀況－

維修事項過多，維修人員不足。


####使用者個案名稱：最新公告

行為者：房東

目標：使房東透過最新公告通知訊息。

前提：有最新公告。

結束狀態：房東已更新最新公告，並回至首頁。

－系列事件：

正常程序－

1.房東透過app進入系統登入成功。

2.房東輸入最新公告。

例外狀況－

沒有任何最新公告。


####使用者個案名稱：房客登錄

行為者：房客

目標：使房客能以會員身份進入大樓管制系統。

前提：房客尚未取得帳密。

－系列事件：

正常程序－

1.房客透過app進入系統登入帳號密碼。

2.系統驗證帳號密碼。

3.系統驗證房客登入成功。

例外狀況－

系統驗證不成功，房客登入失敗。


####使用者個案名稱：門禁感應

行為者：房客

目標：使房客以nfc功能感應進入大樓門禁。

前提：房客手機有nfc功能，並輸入密碼。

結束狀態：進入大樓以及房間後，回至首頁。

－系列事件：

正常程序－

1.房客透過app進入系統登入成功。

2.房客感應成功。

例外狀況－

感應失敗，用密碼輸入進去。


####使用者個案名稱：水電費帳單

行為者：房客

目標：使房客利用app查詢當月水電費及歷史紀錄。

前提：已使用水電。

結束狀態：看完當月水電費，回至首頁。

－系列事件：

正常程序－

1.房客透過app進入系統登入成功。

2.房客查詢水電費。

例外狀況－

還未使用水電至當月底，或是房東尚未完成輸入水電費。


####使用者個案名稱：設備維修

行為者：房客

目標：使房客能以app通知房東需要維修設備。

前提：有需要維修事項。

結束狀態：輸入完需要維修事項，並回至首頁。

－系列事件：

正常程序－

1.房客透過app進入系統登入成功。

2.房客輸入需要維修事項。

3.等待房東回應。

例外狀況－

沒有需要維修事項。


####使用者個案名稱：最新公告

行為者:房客

目標：使房客透過最新公告通知訊息。

前提：有最新公告。

結束狀態：觀看完最新公告，回至首頁。

－系列事件：

正常程序－

1.房客透過app進入系統登入成功。

2.房東或樓管輸入最新公告。

3.房客查詢最新公告。

例外狀況－

沒有最新公告


###強韌圖：
![image](https://cloud.githubusercontent.com/assets/22367717/21960442/be3b1cd2-db26-11e6-9367-01ffcb6f3047.jpg)
![image](https://cloud.githubusercontent.com/assets/22367717/21960441/be16899e-db26-11e6-9b8f-09e9b4b61b8a.jpg)

###循序圖：
![image](https://cloud.githubusercontent.com/assets/22367717/20754908/0412f188-b748-11e6-89cd-a649dc943549.png)

###循序圖REF：
![image](https://cloud.githubusercontent.com/assets/22367717/20754909/0413b2bc-b748-11e6-964c-58e3c84da8e5.png)

###類別圖：
![image](https://cloud.githubusercontent.com/assets/22367717/21359206/6b30125a-c716-11e6-8f93-1fb8f4e6a53c.png)

##APP製作草圖：
###登入帳號：
![image](https://cloud.githubusercontent.com/assets/22367717/21960368/84420994-db23-11e6-94b7-95ead039090e.png)
###房東：
###登入後首頁：
![image](https://cloud.githubusercontent.com/assets/22367717/21960446/f7167e5c-db26-11e6-97c9-44468588aac4.png)
###門禁感應管理：
![image](https://cloud.githubusercontent.com/assets/22367717/21960369/8444e47a-db23-11e6-83cc-48e9286beccd.png)
![image](https://cloud.githubusercontent.com/assets/22367717/21960370/844c85d6-db23-11e6-92bb-92196d5082d1.png)
###水電費管理：
![image](https://cloud.githubusercontent.com/assets/22367717/21960364/79fc424c-db23-11e6-9b30-b72b74fb0bd4.jpg)
###設備維修管理：
![image](https://cloud.githubusercontent.com/assets/22367717/21960365/79fe76c0-db23-11e6-94df-b9f1a77b7a5d.jpg)
###最新公告管理：
![image](https://cloud.githubusercontent.com/assets/22367717/21961133/69c02cc2-db3c-11e6-9a3e-d06452958b51.png)
###房客：
###登入後首頁：
![image](https://cloud.githubusercontent.com/assets/22367717/21960445/f7126312-db26-11e6-8895-c2cc9eb2ef8e.png)
###水電費帳單：
![image](https://cloud.githubusercontent.com/assets/22367717/21960363/79f536dc-db23-11e6-8d1c-48aea96e746f.jpg)
###設備維修：
![image](https://cloud.githubusercontent.com/assets/22367717/21960366/79ffdc5e-db23-11e6-82fb-b81be5f66c60.jpg)
###最新公告：
![image](https://cloud.githubusercontent.com/assets/22367717/21961136/8361c5fa-db3c-11e6-9e31-2c568ff39a8b.png)
####擁有樓管權限：
![image](https://cloud.githubusercontent.com/assets/22367717/21961127/629e9b18-db3c-11e6-9916-726b4c8f37a9.png)
![image](https://cloud.githubusercontent.com/assets/22367717/21961132/6997b738-db3c-11e6-8d7d-91a2904a437a.png)
