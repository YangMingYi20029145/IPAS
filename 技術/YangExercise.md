### 網路通訊安全
### 1.1網路安全(Network Security)
### 網路協定[基礎篇] OSI 7 層 vs TCP/IP 協定組
```
[7]網際網路中主要的通訊協定模式有兩種 OSI 7 層及 TCP/IP 協定組，
請問在這兩個通訊協定模式中，負責傳輸封包（Packet）及選擇路徑（Routing），是那一層的工作？ 
(A) 實體層（Physical Layer） (B) 資料鏈結層（Data-Link Layer） 
(C) 網路層（Network Layer） (D) 應用層（Application Layer）
```
```
C

(一) 實體層 (Physical Layer)
訂定電腦連接的電氣特定協定
功能 :1.讓資料可經由傳輸媒介   2.兩個實際相連的機器間傳送的
例子 :實體層介面有EIA RE-232、RS-449等，而常見區域網路則有乙太網路、記號環、分散式光纖數據介面、CCITT X.25分封網路、整體服務數位網路、同步光學網路等。

(二) 資料鏈結層 (Data-Link Layer)
訊框 (frame) 與實體位置 (MAC)
分為兩個子層：
(一)邏輯連結控制(Logical Link Control, 簡稱LLC)：訊框遞送、錯誤通知、資料流控制
(二)媒介存取控制(Media Access Control, 簡稱MAC)：定義傳輸媒體存取的方式，如CSMA/CD、Token Ring等
例子 ：Physical Address、OSI規定網路上各乙太網路、記號環網路、橋接器等都是在此層運作的。

(三) 網路層 (Network Layer)
邏輯定址
資料封包 (packet) 的傳輸路徑(Routing)選擇
功能：1.決定移動資料的最佳方式(RIP、EIGRP、OSPF) 2.資料遶送 3.錯誤控制(少用)
例子：IP、IPX、路由器

(四) 傳輸層 (Transport Layer)
提供可靠或不可靠的遞送
重傳之前先校正錯誤
功能 ：封包順序、資料流量控制、偵測重複的封包、緊急資料的傳送、複雜的錯誤與回復處理、以及安全方面的課題。
例子 ：TCP 、 UDP

(五) 交談層 (Session Layer)   
負責建立、管理、以及終止兩個通訊主機的對話
功能 ：使不同應用程式的資料與其他應用程式的資料分開
例子 ：SQL 、 RPC 

(六) 表現層 (Presentation Layer)
處理不同資料格式之間的字碼轉換及編碼及解碼
功能：字元碼轉換  資料形態轉換  對資料進行壓縮和加密﹐以提高速度和增加安全性
例子：ASCII 碼和 EDCDIC 碼之間的轉換

(七) 應用層 (Application Layer)
提供使用者介面
功能：檔案、印表、訊息、資料庫、應用服務
例子：HTTP 、 Telnet 、 SMTP 、 POP3 、 FTP 、 SNMP

```
