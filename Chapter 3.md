# 部署的順序
## Apple 產品導入流程以及簡化手段

理解Apple 提供給企業與教育界使用的方案後，讓我們看看具體導入的流程吧。 
這裡將告訴你多數人最常遇到的問題，從購買到初始設定的重點所在。

### 導入流程

STEP 1 - 事前準備
購買 Apple 產品以及取得 D-U-N-S（鄧白氏）認證號碼

STEP 2 - 註冊組織
註冊 ABM / ASM 並且 通過 Apple 審核

STEP 3 - 設定 ABM/ASM
製作管理式 Apple 帳號以及建立新帳號

STEP 4 - 連結 MDM 服務
串接 MDM 工具以及與「自動裝置註冊」的裝置連結

STEP 5 - 進行基本設定
註冊使用者以及一次購買內容並且分發

## STEP 1 - 事前準備
### 購買 Apple 產品以及取得 D-U-N-S（鄧白氏）認證號碼

#### 推薦使用「自動裝置註冊」
當在大量部署 iPhone、iPad 與 Mac 等 Apple 產品時，推薦使用 Apple 所提供輔 助部署機制「自動裝置註冊」來省時省力。可以透過支援「自動裝置註冊」的通路 窗口，或者支援「自動裝置註冊」的 Apple Store 都可以，但請在購買前確認其是否 支援「自動裝置註冊」。購買以後，就會提供給你「Apple 客戶編號」或者「經銷商 編號」來註冊使用。
![Apple Retail](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/0800-095-988.png)
直接從 Apple 購買時，可透過免付費電話（ 台灣 0800-095-988）取得「Apple 客戶編號」。
https://www.apple.com/tw/retail/business/

![Apple Automated Device Enrollment](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/HT204142.png)
從 Apple Store 或支援「自動裝置註冊」的授權經銷
商購買硬體時會提供給你「經銷商編號」。
https://support.apple.com/zh-tw/HT204142

#### 取得鄧白氏認證號碼
可以與購買 Apple 產品同步進行的事前準備手續包括取得鄧白氏（D-U-N-S：The Data Universal Numbering System）號碼。這是 1962 年由 D&B（Dun and Bradtreet）所 開發的九碼企業識別號碼，可以透過它來確認全世界的企業與法人團體。ABM 以及 ASM 都透過這固定號碼來識別個別組織。可以與當地鄧白氏直接聯絡付費申請。其實 也可以透過 Apple 開發者服務（Apple Developer Program）來免費取得號碼，需要以 英文和鄧白氏公司進行聯絡確認各事項，時間約為二至三週。新申請鄧白氏號碼時， 按照組織形態的不同，所需要準備的文件會有所差異。

![D-U-N-S website](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/D-U-N-SNumber.png)
在台灣若要直接申請鄧白氏號碼，可和鄧白氏接洽
付費申請。 
https://dunscertified.dnb.com.tw

![Apple Developer D-U-N-S Number](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/dunscertified.png)
Apple 開發者服務也可以申請鄧白氏號碼。
https://developer.apple.com/support/D-U-N-S/

## 註冊組織
### 註冊 ABM / ASM 並且通過 Apple 審核
### 通過 Apple 的審查吧
購買 Apple 產品之後，企業就要註冊 ABM，學校則是註冊 ASM。手續都是透過網頁瀏覽器於線上到入口網站進行即可。所需要準備的資料就是：申請組織的資訊以及 與 Apple 訂立契約的負責人的聯絡方式。Apple 會透過所提供的負責人電話號碼或郵件位址進行確認聯絡，所以由負責人本人來進行登記設定會最為直接完善。 註冊審查時間最長不會超過五個工作日，會於平日早上九點到晚上五點營業時間內進行電話上的確認聯絡，所以請要有接電話的心理準備。如果沒有缺少任何資料或錯誤的話，就會將審核結果透過郵件寄送，在一個禮拜之內就可以完成註冊手續。

#### 註冊 ABM
![Apple Business Manager login](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Apple%20Business%20Manager%20login.png)
以註冊 ABM 為例進行說明。首先到 ABM 網站點擊「立即註冊」https://business.apple.com

#### 輸入申請資訊
![Registeration form](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Registeration%20form.png)
逐次輸入「姓氏」、「名字」、「工作電子郵件」「企業名稱」，「網站」並選擇是否要收到「Apple 商務必備」的相關新聞和更新資訊，然後選取「繼續」。

#### 建立帳號
![Create account](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Create%20account.png)
建立並確認新帳號的新密碼，然後選取區碼，並輸入你的電話號碼。

到這邊就完成了 ABM / ASM 的註冊並且可以開始使用，但是當你登入時會發現很多功能不能夠使用，這些是因為 Apple 還沒有驗證，當驗證完成後就可以使用 ABM / ASM 的所有功能。

#### 登入 ABM / ASM
![Apple Business Manager login](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Apple%20Business%20Manager%20login.png)
使用先前建立好的帳號登入 ABM / ASM。

#### 驗證組織資訊
![機構設定](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Organization%20Setting%20.png)
前往機構設定，並選取「驗證」。

#### 輸入組織資訊
![機構資訊](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Organization%20Info.png)
逐次輸入「組織名稱」、取得的「D-U-N-S 號碼」、「電話號碼」（代表號等）「首頁網址」，

#### 輸入驗證聯絡人資訊
![驗證聯絡人資訊](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Contact%20Info.png)
輸入組織代表者的名字以及郵件位址、職稱等。完成以後點擊「繼續」。

#### 以郵件通知審查狀況

開始進行審查，就會收到來自 Apple 的郵件。審查最多會花上五個工作天，如果中間遇到週末，大致會需要一個禮拜的時間。

#### Apple 來電確認
平日工作時間會收到來自 Apple 窗口的來電。如果登記的電話沒有人接聽，就會寄送郵件來提醒。

#### 電話中主要會針對這幾點進行確認
1. 登記的身份是否為本人？
2. 是不是 ABM / ASM 的設定管理負責人？
3. 登記的電話號碼與首頁網址是否正確？
4. 使用的目的是為了管理公司裝置嗎？

待確認完成後就可以享受 ABM / ASM 的全功能了。

## 設定 ABM / ASM 
### 建立管理式 Apple 帳號
第一次登入後，管理式 Apple 帳號只有一組登記在公司下頭，後續最好追加其它的管理者帳號，並且幫員工或者教職員等建立管理式 Apple 帳號。這時為了不和一般所使用郵件位置重複，而會給予加上子網域名「appleaccount」的 Apple 帳號。但是為了同仁在登入時更加方便，可以透過「驗證網域」功能驗證組織所希望使用的網域，後續在建立其他的 Apple 帳號時即可選擇組織網域並進行建立，未來使用者登入時也不需要再額外記住另一組網域。

#### 新增網域
![管理式 Apple 帳號](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/add%20domain.png)

前往管理式 Apple 帳號，並選取「新增網域」。

#### 輸入網域
![輸入網域](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/type%20domain.png)
在欄位中輸入組織希望使用的網域，輸入完成後選取「新增網域」。

#### 驗證網域
![驗證網域](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/verify%20domain.png)
網域新增完成後即可在清單中查看到剛才所新增的網域，選取「驗證」。

#### DNS TXT 紀錄
![TXT 紀錄](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/DNS%20TXT.png)
畫面中所出現的 TXT 紀錄必須要新增至網域管理的 DNS 設定中，當新增完成後選取「驗證」即可。


#### 新增帳號
![新增帳號](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/add%20account.png)
要新增管理式 Apple 帳號，請於側邊欄選擇「帳號」於最右側欄位左上角選曲「＋（新增）」按鍵。

#### 輸入姓名與使用者名稱
![Account information form](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Account%20info.png)
輸入新帳號的姓名以及受管理 Apple 帳號的使用者名稱，以及職稱和實際在使用的郵件位址後按下「儲存」。

### 管理式 Apple 帳號的功能與機制
管理式 Apple 帳號，是限制一般 Apple 帳號 可使用的一部分功能後， 供組織專用的 Apple ID。公司的話用來配發給員工，學校則是用來配發給教職員、學生與兒童等。管理式 Apple 帳號好處在於，組織內所使用的 Apple 帳號可由管理者一次設定、管理、針對個別管理式 Apple 帳號設定職務與權限。例如，教師可以透過「大量購買」機制購買 App 或者電子書，對學生、兒童的管理式 Apple 帳號進行密碼重設等。此外，管理式 Apple 帳號當拿到帳號的使用者輸入錯誤密碼 10 次時，帳號就會被鎖定。

管理式 Apple 帳號與其他的 Apple 帳號一樣，可以用於登入配發給個人或者共用的裝置。此外，若是教育機構使用的話，則可以用來
取各式各樣的 Apple 雲端服務，如 iCloud（照片與備忘錄、行事曆
等）、iTunesU 教育服務、使用 iWork 的協同工作功能等。不過需要
注意，為了確保其安全性，管理式 Apple 帳號也有所限制，有些服務
與功能不能使用（如下表）。

企業與學校導入 Apple 產品時，不一定要為每一位職員以及教
職員、學生、兒童配發管理式 Apple ID，但要是能活用這機制，可
以更加確保終端使用者的隱私權以及對組織資安進行保障，更能夠
有效利用導入的裝置。

### 管理式 Apple 帳號不能使用的功能與服務
* 購買 App Store, iTunes Store, Apple Books 內容（但可以瀏覽）
* Apple Pay
* 尋找（舊稱尋找我的iPhone、Mac、朋友）
* iCloud 信箱、iCloud 家庭共享
* 接續 HomeKit 裝置
* 鎖定備忘錄

## 連結 MDM 服務
### 整合 MDM 服務以及與「自動裝置註冊」的裝置連結
### 挑選 MDM 服務並且進行初始設定

購買完 Apple 產品，也完成 ABM 或 ASM 的設定後，就要進入將裝置配發給終
端使用者的階段了。這一階段最為重要的工作，就是在配發前幫裝置進行初始設定
（Kitting）。要讓終端使用者可以立即以裝置進行各項工作的話，就需要基於使用政策來對裝置進行設定。
為了完成這項工作就需要 MDM 工具。選擇一款對自己組織最合適的 MDM 工具
後就要註冊到 ABM 或 ASM 系統中。 然後透過 MDM 工具註冊各個透過「自動裝置註冊」購買的裝置，就可以讓 MDM 與各裝置進行連結。

本部分將使用 Apple 產品管理首選解決方案 Jamf Pro 為例進行說明。

#### 挑選 MDM 服務
![Jamf Website](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/jamf.com.png)
挑選 MDM（行動裝置管理）服務。MDM 提供商每一家的服務內容、價格與支援內容都不一樣，需要按需求詢價後選出最適合的方案。

#### 連結 MDM 伺服器
![Apple Business Manager](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Apple%20Business%20Manager-1.png)
登入 ABM 或 ASM 後，選取側邊欄中的姓名後選擇「偏好設定」，在 MDM 伺服器右邊選擇「新增」

#### 登入 MDM 服務
![Jamf Pro Login Window](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Jamf%20Pro%20Login%20Window.001.png)
到 MDM 服務網頁輸入使用者帳號與密碼後登入。如果使用 Jamf Pro 的話，畫面會如圖所示。

#### 由設定選擇「自動裝置註冊」
![Automated Device Enrollment](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Automated%20Device%20Enrollment.png)

#### 下載公鑰
![Download Public Key](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Download%20Public%20Key.001.png)
顯示自動裝置註冊的設定畫面後，點擊右上角的「公鑰（Public Key）」， 就會下載副檔名為「.pem」的憑證檔案，會存放到「下載」檔案夾。

#### 上傳公鑰
![Upload Public Key](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Upload%20Public%20Key.013.png)

#### 儲存 MDM 伺服器設定
![Save MDM Server settings](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Save%20MDM%20Server%20settings.001.png)
公鑰上傳完畢以後， 點擊右下「儲存」按鍵。之後就會將透過公鑰取得的 MDM 伺服器資訊儲存在 ABM 或 ASM 系統中。

#### 下載 ABM/ASM 的權杖
![Download ADE token](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Download%20ADE%20token.001.png)
接著要發行 ABM/ASM 的權杖 （Token）。 畫面點擊 「下載 MDM 伺服器代號」，就會將副檔名為「.p7m」的憑證檔案下載到「下載」檔案夾中。

#### 上傳 ABM/ASM 的權杖
![Upload ADE token1](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Upload%20ADE%20token1.001.png)
回到 MDM 服務的「自動裝置註冊」畫面，點擊「新增」按鍵。設定「顯示名稱」後點擊「上傳伺服器權杖檔案」。
![Upload ADE token2](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Upload%20ADE%20token2.001.png)
跳出視窗後點選「選擇檔案」，到「下載」檔案夾中選擇剛才下載的 ABM/ASM 權杖Token，點擊「上傳」。

#### 完成伺服器註冊
![ADE Information in MDM](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/ADE%20Information%20in%20MDM%5D.001.png)
上傳完畢後，MDM 服務就會顯示伺服器的識別碼（UUID）以及管理者 ID 和組織資訊等訊息。

#### 完成權杖交換
![ADE Information in ABM](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/ADE%20Information%20in%20ABM.001.png)
這樣就完成 ABM / ASM 和 MDM 服務間的權杖交換，當需要修改資訊或者變更設定時，請到 ABM / ASM 的此畫面進行。

#### 輸入購買通路資訊
![Device suppliers](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Device%20suppliers.001.png)
於 ABM/ASM 的「偏好設定」畫面選擇「MDM 伺服器指派」，於客戶編號右邊選擇「編輯」並輸入「Apple 客戶編號」（從 Apple Store 購買的話），或者「經銷商編號」（於電信商、Apple 授權企業／教育經銷商購買）來進行註冊。

#### 指派裝置
![Assign Devices](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Assign%20Devices.001.png)
點擊側邊欄的「裝置」，並且在裡面選擇想要進行「自動裝置註冊」的設備，點擊右上角按鈕，選擇「編輯裝置管理服務」，並且在清單中選擇要分配給哪一個 MDM 伺服器。

## 進行基本設定
### 註冊使用者以及一次購買內容並且分發
#### 一次部署各種設定
這是最後一個步驟，將使用 MDM 工具來部署初始設定，讓我們從了解 ABM 或
ASM 最基本的設定方式開始吧。

首先得要針對使用裝置的成員設定「職務」。以 ABM 為範例，一般對員工的管
理或者裝置的管理，分發 App 等，都會由多數人擔任管理者，在 ABM 上頭，就有「成員經理」、「裝置註冊經理」、「內容經理」等職務，分別有著不同的權限。此外，當分公司、店面、工廠等有著多數據點時，也可以進行「位置」的設定，更可以對應環境來分配內容。ASM 也可以使用相同的思維方式配置，另外還有供學生、兒童分組的「教室」需要進行設定。

### 設定職務
#### 確認各職務的權限
![ABM Roles](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/ADE%20Information%20in%20ABM.001.png)
這裡以 ABM 作為範例解說。點擊側邊欄「權限管理」中的「職務」可以確認各職務所具有的權限。

#### 管理者職務
![Content Manager](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Content%20Manager.001.png)
以「內容經理」為例，可以使用管理式 Apple 帳號來購買 App 以及電子書。而「裝置註冊經理」能夠進行「自動裝置註冊」，但不能買 App。

#### 幫助使用者賦予職務
![Add Roles](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Add%20Roles.001.png)
在「帳號」欄新增的使用者處可以賦予各種職務。點擊「編輯」按鍵可以變更調整權限。

---
### 購買內容
#### 搜尋想要大量購買的 App 
![App purchase](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/App%20purchase.001.png)
想要購買 App 或者電子書的話透過左邊選單中的「App 與電子書」（臺灣沒有電子書）進行。透過搜尋欄輸入關鍵字。

#### 購買許可
![Google App](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Google%20App.001.png)
這裡以免費的「Google」App 為例進行說明。選擇 App 後於右側欄會顯示「購買許可」等資訊。
*購買付費 App 的話，組織需要預先準備購買的經費*

#### 指定數量與配發目標
![Assign license](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Assign%20license.001.png)
內容經理可以在這裡可以決定購買的數量以及想要配發的「位置」等。確認總金額後點擊「取得」。

#### 購買完成
![Purchage complete](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Purchage%20complete.001.png)
購買完成後可以在App 一覽看到「可以使用 100」，透過「管理許可」畫面可以將App 分發到不同的「位置」。

#### MDM 接收資訊
![MDM App Catalog](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/MDM%20App%20Catalog.001.png)
App 的資訊會自動傳送到所註冊的 MDM 服務。Jamf Pro 的話則可以透過「行動裝置 App」來進行確認。

#### 一次配發更簡單！
![App distribution](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/App%20distribution.png)
如果透過 MDM 進行管理的話，不需要使用個人 Apple ID 等也可以一次配發到各裝置上頭。用來配發組織所使用的 App 非常方便。

### 設定「位置」
#### 管理多個位置
![Location management](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Location%20Management.png)
當有多個辦公室時， 可以從「位置」進行管理設定。如果有需要的話可點擊「新增位置（＋）」來增加。

#### 根據位置不同製作內容代號
![VPP Token](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/VPP%20Token.png)
若有多個位置的話，可由「偏好設定」中「付款與帳單」下載各自的內容代號。當位置需要部署 App 時，就以此進行兌換。

#### 將授權傳送到各個位置
![Locations](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Locations.png)
設定完位置以後， 透過「大量採購」機制買到的 App 就可按位置別分配授權。可以在位置間轉讓授權，也可以委讓授權管理的量。

### ASM 的狀況
#### 設定班級
![ASM Classroom](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/ASM%20Classroom.png)
從側面欄選擇「班級」，就會顯示註冊的班級一覽。班級可以按照科別不同製作，並且可以登錄位置以及教師資訊。

#### 確認學生、兒童的資訊
![ASM Users](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/ASM%20Users.png)
可以為學生、兒童發行各自的使用者編號以及管理式 Apple 帳號，可以透過 MDM 以 CSV 檔案一次上傳所有的教室資訊。

### 一次註冊「教室」資訊
#### 設定第一次的 SFTP 上傳 
![Data source](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Data%20source.png)
ASM 可以透過 SIS / SFTP 來上傳教職員、學生、兒童以及教室資訊。登入 ASM 後，點擊左下角的名字，從「偏好設定」中點擊「管理式 Apple 帳號」，再到「目錄同步」中點擊「開始使用」。

#### 以 CSV 範本來處理資料
![SIS/SFTP](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/SIS_SFTP.png)
就會提供給你 SFTP 的 URL、使用者名稱和密碼，利用此資訊於 SFTP 客戶端設定，同時可以下載 CSV 範本， 一共有位置、教室、學程等六種可供參考使用。

#### 上傳到 SFTP
![Upload with SFTP](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Upload%20with%20SFTP.png)
將這六個 CSV 檔案透過 ZIP 格式進行壓縮後，連結到 SFTP 伺服器，然後上傳
到「Dropbox」檔案夾。上傳完畢後點擊透過 ASM 中「確認 SFTP 資料」來看是
否有錯誤，也可以進行帳號與教室資訊的預覽。

#### 分配權限給教職員
![Assign role](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Assign%20role.png)
製作完管理式 Apple 帳號後，可配發給教職員用於登入。也可以給予各自所需要使用的職務。

### 預先將裝置註冊到 MDM
Jamf Pro 有著「PreStage Enrollments（預先註冊）」的功能。這功能是將裝置的設定存放在 Jamf Pro 中，當要對各裝置進行初始設定時就可以直接套用。若要使用「PreStage Enrollments（預先註冊）」的話，就如迄今為止的說明，將「自動裝置註冊」與 Jamf Pro 連結後就可以使用。此外，關於 Jamf Pro 各種管理功能的詳細說明請見第 18 頁後。
![Jamf Pro Prestage Enrollment](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch3/Jamf%20Pro%20Prestage%20Enrollment.png)
Jamf Pro 可以透過側面欄的「PreStage Enrollments」 來讀取透過「自動裝置註冊」配置裝置的設定。

