
<p class="lead">你將在課堂中，從零開始獨立完成 IoT server 的實作，並同時佈署離線版與雲端版。</p>

課堂將步驟式引導：認識網路拓璞，並為 IoT server 加入 Gateway 與 Broker 的架構，讓物聯網更易於串接 Mobile App。此外，也會認識 CoAP 協定與 HTTP/WebSocket 的差異，學會如何撰寫更省電的 IoT 軟體。

### 課程大綱

> 在 real-time dashboard 的底層，IoT 裝置如何傳送 sensor data 到雲端，並串接 web frontend 呢？這門課程，使用 Web of Things 架構，以及 WebSockets、CoAP 與 Web of Things 通訊協定，來培析 IoT network 的基礎技術，並了解如何建立低耗電的無線感測器網路（Wireless Sensor Networks）。

有別於傳統的 M2M 做法，本課程將以 Web of Things 的觀念（Broker 架構與 URL Routing 觀念），來實作 M2M (Machine-to-Machine)。

* 第 1 課：IoT Network 拓璞架構
 * Wireless Star Network 架構
 * Wireless Ad hoc Network 架構
 * 認識 IoT broker 與 Sensor Gateway<br /><br />
* 第 2 課：IoT broker 與 M2M 實作
 * 使用 CoAP 與 WebSocket 通訊協定
 * 認識 CoAP 與 WebSocket 協定的差異
 * 認識 Broker 架構與 MQTT
 * 使用 IoT Broker 與 URL Routing 實作 M2M
 * Azure 雲端佈署<br /><br />
* 第 3 課：IoT broker 與 CoAP 協定進階
 * CoAP 與 REST 架構比較
 * CoAP 封包解析
 * 低耗電與 Constrained Device 技術解析

### 理念

這門課程是「IoT Network」的入門課程，講師以手把手帶你實作一個完整的「低耗電無線感測網路」。如果你從未學習過「IoT 網路架構」，這門課對是你必修的課程。

無線感測網路（Wireless Sensor Network）最基本的網路拓璞稱為 Star Network（星狀網路），另一個重要的網路拓璞為 Wireless Ad hoc Network（WANET）。這門課帶你從認識 Star Network 開始，動搭建 Star Network 的無線感測網路。

### 課程說明

Star Network 是無線感測網路的基本架構，而 Star Network 架構裡，最重要的硬體稱為 Gateway Sensor Node，在現今的 IoT 網路中，Gateway Sensor Node 也稱為 IoT broker。<span style="border-bottom: 1px solid #da443e;;">這個觀念就是這門課程的名稱由來</span>。這門課程會以 Star Network 建構無線感測網路，並且詳細剖析 ioT broker 的設計與實作。

WSN (Wireless Sensor Network) 是由 *nodes* 所構成的網路架構[2]。在 Sensor Network 裡的 *node* 負責收集資訊，並與其它 *node* 溝通[2]。因此，這個專案要解決的問題有 2 個：

* 如何收集並傳送 sensor data
* node 與 node 間如何溝通，也就是 M2M (machine-to-mahchine) 或 P2P (peer-to-peer) 技術

![](https://upload.wikimedia.org/wikipedia/commons/2/21/WSN.svg)

圖 1: Wireless Sensor Network (Source: https://en.wikipedia.org/wiki/Wireless_sensor_network. License: Public Domain)

Wireless sensor network 的拓璞 (topologies) 之一，就是 Star Network[3]。在 Star Network (星狀網路) 架構中，每一個 *node* 都連接到 Gateway Sensor Node。在 Star Network 裡的 node 會將收集到的資訊，傳送給 Gateway Sensor Node。這個專案將使用 Star Network 架構，因此，除了上述的 2 個問題外，還要再解決另一個問題：

* 佈署 Gateway Sensor Node

![](https://upload.wikimedia.org/wikipedia/commons/8/84/Star_Topology.png)

Figure-2: Star Network (Source: https://en.wikipedia.org/wiki/Star_network. License: CC BY-SA 3.0)

此外，本課程將使用 WebSocket/MQTT/HTTP/CoAP 協定來進行資料傳輸與硬體串接，並分析這些通訊協定的差異，以及 CoAP 如何針對 constrained devices 實現低耗電的技術原理。

### 學習藍圖

根據以上的說明，本課程將帶你實作一個完整的 Wireless Sensor Network。如下圖所示：

* 使用 ESP8266 擷取 real-time 溫度數值
* 使用 ESp8266 擷取 real-time 空氣品質數值
* 以 CoAP 協定串接 IoT broker (Proxy)
* 以 WebSocket 與 HTTP 協定串接 Azure 雲端
* 整合雲端與 Web App

![](https://cloud.githubusercontent.com/assets/1126021/13871103/b0f09960-ed1c-11e5-810b-33f4aa8f0e70.png)

* *架構面*：你將認識 Web of Things、Star Network、IoT Gateway 與 IoT broker 的架構觀念
* *實作面*：你將學習如何修改 IoT broker 的程式碼，並加入解析通訊協定，以及 M2M (machine-to-mchaine) 的新功能
* *技能面*：你將會學習 Azure 的雲端佈局、修改 Node.js 範例程式碼、修改 React 前端範例程式

### 課程對象

* 對 IoT 網路架構規劃有興趣的初學者
* 對使用 Node.js 開發 IoT broker 與 gateway 有興趣的初學者
* 想了解通訊協定如何實現低耗電的技術人員

### 講師團隊

<div>
<img src="https://avatars1.githubusercontent.com/u/1126021?v=3&s=400" width="128" height="128" class="img-circle img-responsive pull-left">
<h6>Jollen Chen </h6>
<p>Jollen，Node.js 全端開發者、Moko365 的技術總監暨講師。正使用 React 與 Node.js 開發 Decentralized IoT 與 P2P IoT 的專案。</p>
</div>

<br >
<div>
<img src="https://avatars0.githubusercontent.com/u/2017447?v=3&amp;s=460" width="128" height="128" class="img-circle img-responsive pull-left">
<h6>Casear Chu</h6>
<p>Casear，對於前後端技術皆有興趣，曾於 Microsoft 與 TrendMicro 任職，於 2012 年獲得 Node.js Knockout 台灣區第一名。曾於 JSDC 2014、2015 擔任講師，也是 SlideNow（線上 Markdown 編輯 Slides）的創辦人。目前興趣轉向 IoT，於 2015 年建立 KitchBot，轉至於廚具的系統分享與建立，並獲得聯發科穿戴式比賽亞軍。</p>
</div>

### 開課時間

* 時間：平日下午班，2 個下午、共計 6 小時
 * Day 1: 2016/10/12（三）14:00-17:00
 * Day 2: 2016/10/13（四）14:00-17:00
* 地點： 台北市博愛路 25 號 3F

