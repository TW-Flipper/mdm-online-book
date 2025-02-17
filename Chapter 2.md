# Apple 詞彙表
## 了解商用、教育所使用的 Apple 專用機制

為了在商務與教育環境更有效率地部署，Apple 提供了各種機制。

只要妥善理解這些知識，就能達到成功部署的結果。

![針對商務、教育的平台全體圖](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch1/Apple%20Full%20Lineup.png)
針對商務、教育的平台全體圖

### 其實很簡單的部署手續

企業與學校在部署 iPhone、iPad 與 Mac 等 Apple 產品時，大致上的流程如上圖所示。在支援「自動裝置註冊」的通路購買產品後，透過 Apple Business Manager 或 Apple School Manager 註冊，再將裝置加入「大量採購計劃」（全名為 Volume Purchase Program、簡稱 VPP）以及 MDM 就好，是可以輕鬆完成的簡單流程。只要理解每個步驟 Apple 提供機制該做什麼事、如何設定，絕對不會複雜難以搞定。

### --- 企業與學校導入產品時必須知道的
# Apple 管理系統的詳細要點

這裡將具體說明Apple 管理機制的每一個項目，不管你是否是系統管理者，只要和 Apple 裝置部署相關，都應該知道這些知識

>**Apple 校務(ASM)**
>更具智慧的管理學校內的裝置與使用者
>-----------------------------
>簡而言之 -> Apple 官方提供給教育機構的入口網站

![Apple School Manager 的登入畫面](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/ASM%20.png)
Apple School Manager 的登入畫面
https://school.apple.com

「Apple 校務（全名為 Apple School Manager、簡稱 ASM）」是 Apple 於 2016 年 3 月推出給教育機構所使用的入口網站。透過 ASM 可以盤點 iPhone 或 iPad、Mac 及 Apple TV 等教育機構內所使用的設備、製作管理組織內成員（教職員或學生、兒童等）的帳號，與 MDM 解決方案進行整合或者購買電子書、App 等授權。當在教育機構使用 Apple 產品時，若要有效活用絕對少不了 ASM。具體的註冊手續與活用方法將於第三章說明。

![ASM 的管理畫面，透過「帳號」增加教職員或者學生、兒童的帳號，「課堂」則可設定學年、班級、「職務」則可指定管理或者教職員、學生等身份。]()
ASM 的管理畫面，透過「帳號」增加教職員或者學生、兒童的帳號，「課堂」則可設定學年、班級、「職務」則可指定管理或者教職員、學生等身份。

>**Apple 商務**
>更具智慧的管理公司內的裝置與使用者
>-----------------------------
>簡而言之 -> Apple 官方提供給企業的入口

![Apple Business Manager 的登入畫面](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/ABM.png)
Apple Business Manager 的登入畫面
https://business.apple.com

相對於教育使用的 ASM，Apple 提供給企業使用的入口網站為「Apple 商務（全名為 Apple Business Manager、簡稱 ABM）」。ABM 一樣透過網頁瀏覽器存取，註冊企業內所使用的裝置，建立、管理組織內成員（員工等）的帳號，與 MDM 服務連結，而能夠完整管理組織內的所有 Apple 產品。若要開始使用，可以先在 ABM 上註冊公司資訊，Apple 再進行資格審查。ABM 具體的註冊手續與活用方法將於第三章說明。

![ABM 的管理畫面。可以對應公司內各級主管的職務設定權限，也可以針對地區設定負責管理的職務。](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/ABM%20Management.png)
ABM 的管理畫面。可以對應公司內各級主管的職務設定權限，也可以針對地區設定負責管理的職務。

>**自動裝置註冊**
>**Automated Device Enrollment**
>自動將裝置至於 MDM 伺服器管理之下
>-
>簡而言之 -> 能大幅減輕設定工作的 Apple 裝置大量管理系統

當企業與學校大量導入 Apple 產品時，得要一台台地進行初始設定 （Kitting） 以及連結到 MDM 服務， 當裝置一多時，對於 IT 管理者來說就增加了非常繁瑣大量的工作。為了讓其變得更為便捷，就可以使用 Apple 所提供的「自動裝置註冊」服務。

在支援「自動裝置註冊」的通路、企業／教育通路購買 Apple 產品時，Apple 或者企業／教育經銷通路會將裝置的序號註冊到「自動裝置註冊」系統中，然後會提供你客戶編號或經銷商編號。管理者可以直接將客戶編號以及經銷商編號連結到 MDM 服務（需要透過「Apple 校務」或者「Apple 商務」先與 MDM 伺服器整合）。

這麼一來，就可以簡單地將所購買的 Apple 產品全部登錄到 MDM 管理之下，透過 MDM 將設定描述檔、App 一次部署，也可以透過發送命令來管理裝置或清除資料。

### 「自動裝置註冊」主要的優點

**1. 減少裝置部署時必要的設定作業量**

可以自動將裝置加入 MDM 服務的管理之下。另外，當要將裝置變更到監管模式（Supervised mode）時，就得需要以有線的方式透過 Apple Configurator 來進行設定。但若使用「自動裝置註冊」的話，就可以無線進行設定。

**2. 精簡啟動步驟**

Apple 產品第一次啟動時會要求你進行各式各樣的初始設定，但若使用「自動裝置註冊」的話，使用者端就不需要進行這樣的過程。第一次開啟裝置後連接到網路就會自動連結到 MDM 服務並加入管理，透過無線接收在 MDM 上所設定好的內容。

**3. 不能解除 MDM 的設定**

過往用來進行裝置管理以及遠端設定使用的 MDM 設定描述檔可以被使用者刪除，刪除以後該裝置就變 MDM 管理的對象外，則需要再次進行設定。若使用「自動裝置註冊」的話，就可以避免 MDM 的設定描述檔遭到刪除，而能加強使用上的安全性。

**4. 強制安裝 MDM**

讓裝置變成不安裝 MDM 設定描述檔就無法使用的狀態。換句話說，只要不使用 MDM 服務就不能夠使用該裝置，而一定得要將裝置置於 MDM 所管理的狀況之下。

### 支援「自動裝置註冊」的 Apple 產品
* 使用 iOS 7 或更新版本的 iOS 裝置
* 使用 iPadOS 的 iPad 裝置
* 使用 OS X Macericks 10.9 或更新版本的 Mac 裝置
* 使用 tvOS 10.2 或更新版本的 Apple TV 裝置(第四代或更新世代)
* 使用 visonOS 2 或更新版本的 Apple Vision Pro

以外的裝置若要加入「自動裝置註冊」的話，需要透過 Apple Configurator 來手動準備

>**行動裝置管理**
>**Mobile Device Management(MDM)**
>安全地管理、使用組織內的裝置
>-
>簡而言之 -> 專門用於管理行動裝置的解決方案

MDM（行動裝置管理）是 Apple 提供用於裝置管理的框架，使用它所打造的的 MDM 工具（或者 MDM 解決方案），
則由其他第三方廠商所提供，讓管理者可以利用來有效率地管理組織內的裝置。
MDM 能做的事情各式各樣，大致上可以分為 

1. 取得裝置資訊（作業系統版本以及安裝的 App 一覽等）、
2. 套用設定部署檔（密碼或者 Wi-Fi、安全政策、App 使用限制與各種設定等）
3. 管理指令（遠端重設與刪除密碼等）

這三個大項目，MDM 實際可以做到的事將於第四章詳細進行說明。

![以提供強大 Apple 產品 MDM 服務而知名的 Jamf Pro 的管理畫面，可以按照組織內如何使用 Apple 產品為基礎，從各式各項角度製作設定描述檔。](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/Jamf%20Pro%20.png)
以提供強大 Apple 產品 MDM 服務而知名的 Jamf Pro 的管理畫面，可以按照組織內如何使用 Apple 產品為基礎，從各式各項角度製作設定描述檔。

### MDM 機制解說

![MDM 機制解說](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/MDM%20Mechanism%20Explanation.png)
MDM 伺服器經由 Apple 的推播通知伺服器（APNS）對裝置送出要求。當裝置的電源沒有開啟或者沒有連接網路，此等無法接收到推播通知的狀況下無法執行指令。遇到這狀況請開啟電源、連接網路，讓裝置能接收通知就可以執行。

## 「自動裝置註冊」與「Apple 校務」、「Apple 商務」、「MDM」之間的關係

企業與學校在使用 Apple 產品時，必須正確地將設備設定好配發給使用者。所以將裝置置於 MDM 管理下是必要的條件。部署 Apple 產品時較不容易理解的，主要是如何將 Apple 產品連結到 MDM 的部分，所以得要知悉「自動裝置註冊」與 「Apple 校務」、「Apple 商務」之間的關係。這裡將介紹使用「自動裝置註冊」與否，在購買裝置後設定工作流程的差別。使用「自動裝置註冊」的話可以大幅簡化部署作業、也可以降低部署上所需的支出。

![「自動裝置註冊」與「Apple 校務」、「Apple 商務」、「MDM」之間的關係](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/Relationship%20Between%20Automated%20Device%20Enrollment%2c%20ASM%20&%20ABM%2c%20and%20MDM.png)

>**大量採購計劃**
>**Volume Purchase Program(VPP)**
>更有效率地購買機構內所使用的 App
>-
>簡而言之 -> 大量購買 App Store 裡 App 的機制

對學校以及企業而言，以何種方法取得 App 是個重要的問題。如果購買的裝置數量不多時，還可以讓使用者個別使用自己的 Apple 帳號從 App Store 取得 App，但在部署大量裝置時，就得要從管理端一次進行配置了。這時如何取得個別 App，而若是收費 App 的話，該以何種方式付費？也是經常讓管理者頭疼的問題。

在 App Store 購買 App 時可以使用信用卡或者電信帳單付費，同樣可以使用法人戶頭的信用卡或者簽帳卡來進行付費，但在發票單據處理上還會造成一些麻煩。而且使用者購買 App 後，權限會與個人的 Apple 帳號綁在一起，若人員調動，可能未來就無法再下載購買的 App，會是個問題。

為了解決這樣的問題，就可以使用「大量採購計劃（全名為 Volume Purchase Program、簡稱 VPP）」機制。只要使用這個機制，管理者就可以一次購買大量 App 的授權，並且指定發佈到不同裝置上頭，可以大量減少購買以及安裝的手續。購買的 App 會與管理者的 Apple 帳號綁定，所以可以回收、再發佈到不同裝置上頭。如果與 MDM 服務連結的話，更可以一口氣對多台設備進行配置。以回收、再發佈到不同裝置上頭。

![大量採購計劃](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/volume%20purchase%20program%20.png.jpg)

>**Apple 帳號**
>和個人帳號不一樣，你一定要知道差異在哪裡！
>-
>簡而言之 -> 使用 Apple 產品與服務必須要有的帳號

「Apple 帳號」是使用 Apple 產品以及服務時必須要有的帳號。個人使用的狀況，自己申請一個 Apple 帳號就可以了事。但是若是企業或者教育機構，如果交給個別使用者申請自己的 Apple 帳號，之後對於裝置、App、內容的管理將會變得相當麻煩。所以若是組織使用的話，最好一開始就由管理者來申請 Apple 帳號較為適切。

不過按照使用方式，也可以不需預先申請 Apple 帳號。可以透過 ASM 或者 ABM 針對各項服務來指定不同的「管理式 Apple 帳號」。例如可以用管理式 Apple 帳號來登入裝置，但是卻和一般的 Apple 帳號不同，不能用它來購買 App、也可以停用 Facetime 與 iMessage 等服務，可以限制能使用的 Apple 服務範圍。

此外，組織內所使用的 Apple 帳號除了給予終端使用者之外，也可以應用於「自動裝置註冊」或「大量採購計劃」等機制，作為使用 Apple 法人、教育系統裡「代表組織」的帳號。管理者得先理解不同 Apple 帳號的定位，然後妥善地納於管理之下。

![Apple 帳號可以透過 Apple 網站建立](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/Apple%20ID.png)
Apple 帳號可以透過 Apple 網站建立
https://account.apple.com/


### 你也應該知道這些名詞！

>連接學生與老師的 App

![課堂](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/Classroom.png)

#### 課堂

與 Apple 校務同時公布供教育使用的 iPad 專用 App。教師端啟動該 App 時，同網路中的學生、兒童所使用的 iPad 都會納入控制之下，可以啟動 App、指向特定的作業、或者透過 AirDrop 傳送檔案。另外還可以進行鎖定畫面、靜音等控制。教室 App 單獨也可以使用，主要是與 Apple 校務相互連結進行管理，可讓 iPad 更適宜用於課堂授業用途。

>出家庭作業、確認完成進度

![課業](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/Schoolwork.png)

#### 課業

功課可配合課堂 App 一起使用，是可用來加強學生、兒童學習體驗的免費 App。功課顧名思義，教師可以從 iPad 中將網頁連結或 PDF、文件或者特定 App 中的活動，簡單地配發到學生、兒童的 iPad 上頭，也可以和學生、兒童進行一對一的溝通，確認其功課的完成狀態來給予指導，也可以針對個別學習狀態量身打造功課。此外，學生、兒童功課的進度與期限都可以在 iPad 上進行管理。


>想要打造專用 App 的話

![Apple Developer Program]https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/Apple%20Developer.png)

#### Apple Developer Program

當組織內要進行 App 開發的話，則必須加入本計畫。只要有 Apple 帳號的話個人也能夠註冊、註冊本身為免費。但如果要透過 App Store 販賣、發送 App 的話， 就必須支付約 99 美元（新台幣 3,400 元）的年費。企業開發的 App 不需要透過 App Store 公布，而是要針對職員為對象開發、部署的話，就可以申請「Apple Developer Enterprise Program」。

>Apple 官方的部署工具(macOS 專屬)

![Apple Configurator](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/Apple%20Configurator.png)

#### macOS 版 Apple Configurator

這是 Apple 透過 Mac App store 所提供的部署設定描述檔的工具程式。可以將設定描述檔檔製作完畢後，利用有線的方式安裝在 iOS、iPadOS 與 tvOS 設備上。 同時能與和「大量採購計劃」相結合， 所以也能管理並安裝 App 在 iOS、iPadOS 與 tvOS 的設備；另外也能將 iOS、iPadOS 與 tvOS 設備加入至「Apple 校務管理」、「Apple 商務管理」中，讓這些設備未來能利用 MDM 系統遠端更新設定。由於這個軟體只能運作在 macOS 上，而且必須與裝置接上線才能更新設定， 比較適合應用於少量設備管理。

>Apple 官方的準備工具(iOS 專屬)

![Apple Configurator](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/apple%20configurator%20for%20iphone.png)

#### iOS 版 Apple Configurator

這是 Apple 透過 App store 所提供的準備工具。可以將 iOS、iPadOS 與 macOS 設備加入至「Apple 校務管理」、「Apple 商務管理」中，讓這些設備未來能利用 MDM 系統遠端更新設定。

>Apple 官方的雲端服務

![iCloud](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/iCloud.png)

#### iCloud

iCloud 是 Apple 所提供的雲端服務，可以用來保存 iPhone，iPad 或者 Mac 等 Apple 產品裡頭的通訊錄、訊息、照片等內容於雲端， 在裝置之間同步、分享。此外 iCloud 還有分享協同的功能，例如「照片」可以設置「共享的相簿」、iWork App（Pages、Numbers 與 Keynote）也可以進行協同作業。iCloud 免費 提供 5GB 的空間，最大付費可以擴充到 2TB 的儲存空間。此外，教育機關則是提供免費 200GB 的空間可以使用。

>更了解 Apple 產品的活用術

![Apple Teacher](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch2/Apple%20Teacher.png)

#### Apple Teacher

這是提供給教師使用的專業學習方案，用來學習或者教導如何活用 Apple 產品。只要有 Apple 帳號的話就可以註冊，透過網頁來學習 Mac 與 iPad、隨附軟體與 App 的相關知識，以及實際使用的技巧與工作流程。Mac 的話則可配合教材如「Mac 版 Pages 使用手冊」、 「Mac 版 Keynote 使用手冊 」 等 iBooks 提供的指南書來學習技巧，更可以直接參考線上協助。完成測驗後就可以會獲得標章，會提供官方徽章來認定你是 Apple Teacher。








