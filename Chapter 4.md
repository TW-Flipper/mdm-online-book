# 活用 MDM
## 完全瞭解 MDM 所能辦到的事

企業與學校如果要部署、活用大量的Apple 裝置的話，就一定要使用 MDM 服務。

接下來讓我們來了解配合MDM，可以做到哪些事情。

### 為什麼一定要 MDM

行動裝置管理（MDM）是為了管理 iOS、iPadOS、tvOS、macOS，由 Apple 所提供的軟體框架。使用透過此框架開發的 MDM 工具，管理者就可以用來做裝置的部署、數位資產的整理、設定、應用程式的管理、刪除資料、維護資安政策等作業，能夠更有效率地管控 Apple 產品。

若要以 MDM 管理裝置的話，就需要將裝置註冊到 MDM 服務之中。註冊方法分為以下四類。

* 自動裝置註冊。
* 描述檔式「裝置註冊」
* 帳號導向的「裝置註冊」
* 帳號導向的「使用者註冊」

主要推薦的方法是使用「自動裝置註冊」機制進行。

### 將裝置註冊到 MDM 的方法

|   | 註冊方法 | 使用者手續 | 監管模式 |
| ------------------ | ------ | --------- | ------ |
|自動裝置註冊          | 自動註冊 |拿到裝置後開啟電源連上網路就會自動設定好 | ✅ |
| 描述檔式「裝置註冊」  | 手動註冊 |透過安裝註冊描述檔加入管理 | ✅（Mac）<br>❌（iPhone、iPad、Apple TV、Apple Vision Pro） |
| 帳號導向的「裝置註冊」| 手動註冊 | 透過在「設定」或「系統設定」中登入「管理式 Apple 帳號」 |✅（Mac）<br>❌（iPhone、iPad、Apple Vision Pro）|
|帳號導向的「使用者註冊」| 手動註冊 |透過在「設定」中登入「管理式 Apple 帳號」 | ❌ |

現在有各式各樣的業者提供 MDM 服務，這裡以最早支援 Apple 各項機制，並且有著眾多特有功能也具備完善支援服務， 並且可以透過統一的機制一併管理 iPhone、iPad、Apple TV、Apple Vision Pro、Apple Watch、Mac 的 Jamf Pro 作為案例進行說明。

### MDM 功能一覽

#### 零接觸部署
連結「自動裝置註冊」的話，第一次開機並連上網路時就可以自動設定／配發指定的設定描述檔／監管模式／連結 AD & LDAP

#### 設定描述檔
設定 Wi-Fi、VPN、密碼政策／ iOS 的功能設定與限制

#### 資產（Inventory）管理
硬體資訊、作業系統資訊、網路 App、已經套用的部署檔、加密／製作報告

#### 遠端命令
遭竊、遺失時刪除資料、上鎖／強制安裝 App 到單一或者多數裝置／作業系統更新／開啟關閉藍牙

#### App 管理
透過「大量採購」採購授權／不用 Apple ID 也可以從公司 App 目錄安裝／分發受管理的 App 以及 AppConfig 檔案／設定不能使用的 App

#### 資安設定
透過設定描述檔建構組織的資安設定／禁止從 App Store 安裝 App ／開啟單一 App 模式／遠端命令

## MDM 的基本功能
### 資產管理
#### 有效率地收集組織內裝置的資訊

資產，英文 Inventory 的意思除了「資產」以外，還包括「目錄」。應用 IT 管理，就是指企業或學校所購買的硬體以及軟體；對 MDM 工具來說，就是指各項資料，如：裝置的型號、序號、儲存容量以及可用容量、UDID（裝置唯一識別碼）、安裝的作業系統版本以及 App 等資訊，都可以透過MDM 工具的管理畫面一目瞭然。

此外裝置的狀態、是否為受監管的對象、安全狀態與 IP位置、已經安裝的設定部署檔、購買資訊等也可以即時確認，如果發現有違反使用政策的裝置，就可以立即對應處理。裝置一台一台由人力進行確認的話，所部署的裝置越多，花的工夫越多越麻煩，透過 MDM 工具自動搜集資訊可以大幅增加管理效率。

Jamf Pro 不僅針對個別裝置搜集資訊，也可以基於資產資料動態生成「智慧群組」，能夠挑出符合多個搜尋條件的裝置，來套用設定部署檔。

![Jamf Pro Search Inventory](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Jamf%20Pro%20for%20Mac%20features.png)
本圖為 Jamf Pro 介面，可以透過各式各樣的搜尋條件來取得資產資料。

### 配發 App 與電子書
#### 遠端配發組織內所使用的App 以及電子書

企業與學校採用 Apple 產品其中一項常見的需求，就是將各式各樣的 App 與電子書安裝到設備上，讓員工或教職員、學生、兒童來使用、閱讀。若在需要的時候將需要數量的 App 與電子書安全地配發到大量的裝置上，就會需要 MDM工具來節省時間與力氣。

選擇 MDM 工具時有一項關鍵， 就是支援哪些種類的內容配發。Jamf Pro 的 話， 不僅支援在 App Store 上販賣的App，也支援 App Store 以外，如微軟以及 Adobe 所提供的付費／免費 App，以及僅為了組織內部使用而開發的 In-House App，還有透過 Apple「大量採購」機制大量購買的App，以及在 Apple Books 上所販賣的電子書。以上都支援遠端派送、更新以及刪除等操作。

當要配發時，直接到 Jamf Pro 新增 App，可以設定派送方式以及設定等項目。挑選接收 App 的使用者或裝置後，看是要自動地安裝到裝置上頭，或者使用「Self Service」 讓使用者自行安裝，都能夠自行選擇。

![Jamf Pro Mobile Device App settings](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Jamf%20Pro%20Mobile%20Device%20App%20settings.001.png)
Jamp Pro 可以從「行動裝置 App」選單挑選要配送的 App。

### 管理命令
#### 處於異地也能遠端強制執行各項工作

採用 MDM 工具最大的優點就是能夠使用「管理指令」。這功能是以部署的裝置為對象，可以透過遠距指令執行各式各樣工作的功能。最具代表性的管理指令就是遠端鎖定和遠端清除，當終端使用者遺失裝置的時候，為了避免洩露機密或者個人資料，而透過遠端指令鎖定螢幕，將裝置內的資料刪除恢復出廠狀態。

除此還有其他功能，例如針對特定裝置或者特定群組更安全設定、傳送通知、修改裝置名稱、開啟／關閉藍牙，還可以重設密碼或這變更桌面圖片等等。

![Jamf Pro Mobile Device Remote Commands](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Jamf%20Pro%20Mobile%20Device%20Remote%20Commands.png)
選擇裝置後，由「管理命令」中選擇命令，就可以遠端對裝置進行操作。

### 設定描述檔
#### 將組織內的各項政策一次配發到所有裝置

設定描述檔是 iPhone 或 iPad、Mac 中所存放的設定資訊檔案。使用 MDM 服務的話，就可以設定各式各樣的預設資訊，配置到受管理的裝置上頭。這可以使得過去非常麻煩的終端用戶設定變得更為順暢，一拿到設備直接設定好。也可以讓管理者基於組織內的管理政策，套用各種限制。不僅應用於裝置的初始設定，配發裝置以後，若管理政策有所變更，也可以遠距更新設定部署檔。

設定描述檔中所包含的內容各式各樣。包括 Wi-Fi 與 VPN、Google 服務（Google Workspace）等帳號設定，也包括 LDAP 等企業目錄服務、分享的行事曆與聯絡人等、也能為瀏覽器加上內容過濾器，這些都能包含在內。

除此之外，也可以對 AirPlay 或 AirPrint 等裝置原有的功能進行限制， 也可支援各種憑證、SCEP 與 ACME 的建構。

![Jamf Pro Mobile Device Configuration Profiles](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Jamf%20Pro%20Mobile%20Deivce%20Configuration%20Profiles.png)
設定部署檔所能包含的資訊多種多樣。本圖為針對裝置採用單一 App 模式時所能指定的各種細節設定。


## Jamf Pro iOS & iPadOS 能辦到的事
### 透過監管模式來詳細管理

iOS、iPadOS、tvOS 與 visionOS 有一項特別模式，就是使用 MDM 伺服器可進行詳細管理的「監管模式（Supervised Mode）」。 若要讓裝置開啟監管模式的話， 就需要透過 Apple Configurator 來先將裝置初始化，或者「自動裝置註冊」的裝置可以透過加入 MDM 服務進入該模式。

開啟監管模式後，可以透過 MDM 來控制 AirDrop 功能，或者不顯示指定的 App等功能，讓管理者可以對裝置進行非常細節的操作。這裡將就 Jamf Pro 代表性的功能進行介紹。

### 客製化 Home 畫面
#### 讓螢幕顯示變得更易於使用

可以將公司的商標或者企業標準色等製作成 Home 畫面的桌布來統一配置，可以統一視覺識別，有效提高品牌認同。同時也可以鉅細靡遺地指定 Home 畫面所置放的 App 及資料夾、Dock 配置等。

舉個具體的例子：將公司所使用的系統及服務，不管是透過 App 或者網頁捷徑，重要的放在第一個螢幕上，而把不重要的 App 移動到第二個畫面後。此外也可以隱藏與業務無關的 App。這樣就不需要左右滑動來尋找 App 在哪兒，單點就可以存取所需要的功能。

![iPad Home screen](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/iPad%20Home%20screen.png)
可以將 「Self Service」 固定放在 Dock 上，調整 App 的配置，以及將電話與設定以外預設的 App 設定為不顯示。

### 單一 App 模式
#### iPad 作為 Kiosk 裝置使用

「單一 App 模式」，是讓 iPad 僅能使用特定功能、當作 Kiosk（自助服務機）裝置使用的模式。也就說把 iPad 當作高性能的觸控裝置來使用。例如餐飲店的點菜裝置或者收銀器材，公司接待處的登記裝置、展覽會的問卷或者客戶意見蒐集裝置等等。（也可以讓觸控功能關閉來做專門展示使用）通常專為了這樣目的開發機器的話，會花上不小的成本以及開發時間，透過「單一 App 模式」以及自家開發的 App，就可以大幅度縮減成本以及時間。

![Jamf Pro Mobile Deivce Configuration Profiles](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Jamf%20Pro%20Mobile%20Device%20Configuration%20Profiles.png)
設定單一 App 模式時，可以針對功能細節，如觸控輸入、畫面旋轉、各按鍵的功能能逐一設定。

### 製作教育用的部署檔
#### 有效率設定共用的 iPad

Jamf Pro 可以基於 ASM 中教職員以及學生、兒童的名冊，加上授課（教室）的資訊，自動產生「教育設定描述檔」，針對所有受管理的 iPad 發送並且套用設定。透過這樣的作法而可以讓「Classroom（課堂）」App 得以應用於協助授課。此外，因為部署了一樣的設定部署檔，而能讓多的學生、兒童共用同一台 iPad，可以切換所配發的管理式 Apple 帳號，IT 管理者可以簡單地開啟使用這項功能。對於教育現場配置多台 iPad 的狀況來說，幾乎是必要的功能。另外可以配合每間學校不同的管理措施，也是一大重要的特點。

![Jamf Pro EDU Profile](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Jamf%20Pro%20EDU%20Profile.png)
使用 Jamf Pro 可以建立教育設定描述檔，配發後可以結合 Classroom 教室 App來使用，簡單地透過新的方式來進行授課。

### 設定課堂 App
#### 減少教職員與學生設定的麻煩

「Classroom（課堂）」這款支援學習 App 雖然可以透過手動建立課堂資料，但如果預先與 ASM 以及 MDM 連結的話，就能夠一口氣將 iPad 的設定部署到多台裝置上直接使用。另外也可以從 ASM 輸出使用者資料到 Jamf Pro 上頭，在 Jamf Pro 製作新的使用者，或者更新既有使用者的資料。這樣可以讓管理端預先整合各方資料，避免教員與學生、兒童花了太多上課的時間在 iPad 設定以及調整上頭。此外透過部署檔，也可以進行教員與學生的群組設定、共用 iPad 的 App 使用限制以及 Dock 的客製化設定。

![Classroom app](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Classroom%20app.png)
讓 ASM 以及 MDM 連結，可以一口氣基於教員和學生的資訊完成各項 iPad 的設定配置，有效節省時間。


## Jamf Pro tvOS 能辦到的事
### 配置於會議室或者醫院

大眾對 Apple TV 的印象，多是接在家裡電視上頭，作為娛樂設施來使用，但其實也可以應用在企業與教育機構中。如可以連結到會議室或者課堂上的電視，透過iPhone 或者 iPad 來進行簡報投影、也可以設置在旅館的課室或者醫院的病房中，有各式各樣的應用方式。企業或學校若要採用的話，管理者還是會遇到手工進行設定與部署所要耗費的時間與力氣、個別 App 的安裝與設定、資產管理等都會是問題，這時使用 MDM 可以有效解決這些麻煩。以下是採用 Jamf Pro 時可以做到的功能。

### 會議室模式
#### 將 Apple TV 自動開啟會議室模式

Apple TV 有一個叫做「會議室顯示器」（以下稱為會議室模式）的功能，可以讓裝置透過 AirPlay 連結來顯示畫面，教室或者會議室可以使用這模式，按照螢幕上顯示的順序，讓 Mac 或者 iPhone、iPad 的螢幕顯示在 Apple TV 所連結的顯示器上，而能立即開始進行簡報。Jamf Pro 可以將會議室模式的設定部署檔一次配送到多台裝置上頭。 並且可以透過設定，自行定義會議室模式時螢幕要顯示的訊息。

![Meeting Room](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Meeting%20Room.png)
從「裝置」頁籤選擇會議室模式的「設定部署檔 」，然後遞送到想要的 Apple TV 上頭。

### 配送自行開發的App
#### 配送數位看板用的 App

Jamf Pro 可以針對 tvOS 所使用的自開發的 App。基本概念以及設定順序與 iPhone 或 iPad 都一樣，Apple TV 可以透過單一 App 模式來作為「數位看板（Digital Signage）」或者公共空間使用的「導覽看板」，也可以允許單一 App 運作作為「Kiosk（自助服務機）」。具體而言，可以在旅館客房的電視顯示原創內容、在醫院的候診室或者銀行交易所得大廳顯示掛號號碼。只要能夠使用 HDMI 連結的顯示器，無論電視還是投影機、大型顯示器都可以使用，可以大幅降低開發成本。

![Jamf Pro Deploy In-House App](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Jamf%20Pro%20Deploy%20In-House%20Ap.png)
可以部署針對 tvOS 自行開發的 App。 對數位看板或者導覽看板來說都很有用。

### 控制 AirPlay
#### 限制 AirPlay 避免意外

使用 MDM 工具，可以針對辦公室或學校等所配置的Apple TV 功能，例如 AirPlay 鏡像功能、影片的串流功能等各種細節進行設定，避免受到預想外的濫用。具體來說可以針對開放／關閉 AirPlay 功能，或者第一次連接時是否一定要輸入密碼。此外也可以決定能透過 AirPlay 連結的裝置是要在同一個網路內，還是可以同意在附近的裝置也能使用。此外，也可以只讓特定的 iOS 裝置連結 Apple TV， 也可以控制 「Apple TV Remote」的連結權限。配合適當的 AirPlay 管理機制，可以安全地部署裝置。

![AirPlay Restriction](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/AirPlay%20Restriction.png)
AirPlay 可以讓 iPhone、iPad 以及 Mac 以無線串流影片或者音樂。MDM 可以針對 Apple TV 的連結方式進行限制。

### 遠端指令
#### 遠隔重新啟動或者刪除資料

和 iPhone、iPad、Mac 一樣，Jamf Pro 可以對 tvOS 進行遠端指令管理。其中包括「重啟 Apple TV」以及「刪除 Apple TV」等項目，使用這些指令可以讓 Apple TV 遠端無線進行復原工作。特別是在醫院或者旅館等使用者會更換的地點，就可以讓 Apple TV 在更換使用者時刪除個人資料，回歸初始狀態。而且不需要管理者個別手工操作進行設定與維護，變得非常方便。

![Wipe devices](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Wipe%20devices.png)
使用 tvOS 的遠端指定，可以讓受管理的 Apple TV 強制執行指定的工作。

## Jamf Pro macOS 能辦到的事
### Jamf 管理 Mac 功能超強

iOS 或者 iPadOS、tvOS 都是透過 Apple 的 MDM 框架來進行管理，所以功能有限。但 macOS 作為電腦系統，在 IT 上需要更多以及更完整的管理功能。

Jamf Pro 需要在 Mac 上安裝「Agent」程式來作為輔助，使用「Agent」能建立隱藏的管理者帳號來進行管理作業。如此一來能夠超過一般 MDM 的限制而對 Mac 做出高層次的管控，可以說是 Jamf Pro 最大的優勢。具體上能對 Mac 做出怎麼樣的控制，請見以下主要功能的說明：

### Jamf Pro 的 Mac 管理功能
![Jamf Pro for Mac features](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/Jamf%20Pro%20for%20Mac%20features.png)
Jamf Pro 除 了 macOS MDM 框架可以做到的事情外，還有著特有的控制功能。

### 具彈性的註冊方式
#### 使用中的 Mac 也可以新增到管理之下

當要部署新的 Mac 時，可以與 iPhone、iPad 和 Apple TV 使用相同的「自動裝置註冊」機制，或者透過 URL 註冊到 Jamf Pro（MDM）伺服器上頭。此外，也可以讓已經部署使用中的 Mac 註冊受到管理。

### 客製化偏好設定
#### 設定使用者權限與設定描述檔

可以對 Dock 上的 App 進行調整，也可以針對系統偏好設定中 Wi-Fi 或 VPN 等項目透過設定部署檔進行設定。另外也可以針對受管理的 Mac 中的使用者權限和設定進行修改、也能新增、刪除帳號。此外也可以讓 Mac 與 Microsoft 的 Active Directory 或者 Apple 的 Open Directory 等目錄服務進行連結、分配。

### 安裝各種驅動程式與App
#### 連結印表機安裝 PKG 檔案

Jamf Pro 可以針對受管理的 Mac 配發 App、進行更新作業，除此之外還可以透過「白名單」功能，讓沒有管理者權限的職員也可以安裝從 Mac App Store 外取得的 App、或者安裝印表機等裝置的驅動程式。另外也可以製作「黑名單」，讓全部或者一部分的使用者能夠無法啟動、安裝特定的 App。

### 資產管理
#### 可以取得超過 MDM 框架的資訊

Jamf Pro 除了前面所介紹能夠取得的資產管理資訊外。Mac 上還能夠獲得本機端使用者帳號、印表機設定、開啟的服務、可以使用的軟體更新、應用程式的使用狀況、安裝的字體、外掛等各式各樣的資訊。

### 支援各種資安功能
#### 支援 FileVault 或 EFI、T2 晶片

可以透過 Mac 標準的磁碟加密功能「FileVault 2」強制進行鎖定並回收恢復密鑰，就算 Mac 沒有 T2 處理晶片支援，也可以啟動 EFI 密碼以阻斷預設啟動磁碟以外的外部開機磁碟。另外也可以管制 iCloud 的使用等，以及利用 Proxy 來管制網路存取。

### 建構 Self Service 服務
#### 在組織內建構自己的 App Store

Jamf Pro 能夠建立僅供組織內部使用的 App Store（App 配送目錄）服務。可以將 App Store 購買的 App、以及組織自己開發的 App、受第三方授權的 App 登錄到系統上，讓終端使用者透過介面來自由地於受管理裝置上安裝。此外，不僅限於 App、也可以將工作上需要的檔案，如書籤檔案、PDF、輔助資料等登錄到該系統中。管理者可以與目錄服務互相整合，與使用者的業務、位置以及職位等結合進行客製化設定、不僅能夠減少到場安裝的工序與成本，也可以提供終端使用者更好的體驗。

![macOS Self Service](https://info.aatp.com.tw/hubfs/MDM%20Books%202025/Ch4/%5BmacOS%20Self%20Service.png)
Self Service 的名稱、圖示、背景等介面都可以透過管理者介面進行客製化，存取時也可以要求登入認證。
