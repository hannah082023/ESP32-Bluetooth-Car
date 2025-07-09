# ESP32-Bluetooth-Car
113-2工科系工創課第12組期末專案。
## 1. 材料準備
* 壓克力板
* L298N*1
* 焊好的馬達*4
* 輪子*4
* NodeMCU-ESP32
* 兩排的電池盒+一排的電池盒 (串連起來用)
* 18690電池*3 (經測試與計算，三顆18690電池串聯為最適合的電壓)
* 電池充電座
* 尖嘴鉗與螺絲起子
* 焊接工具
* Micro-USB傳輸線 (必須有傳輸功能)
## 2. 電腦環境建置
* 使用Arduino IDE
* 開發板管理員：esp32 by Espressif Systems ver. 2.0.16
* 程式庫：DabbleESP32
* (可能需要) 驅動程式: CP210x
## 3. 上傳Code (HannahCar.ino)
車子藍牙名稱：HannahCar  Board: DOIT ESP32 DEVKIT V1  Upload Speed: 115200
記得選序列埠，沒有偵測到的話裝驅動程式或換一條線
## 4. 組裝與接線
(1) 電池盒接L298N
* 正極接12V
* 負極接GND
(2) ESP32接L298N
* VIN接5V
* GND接GND
* D18接IN3
* D19接IN4
* D25接IN1
* D26接IN2
* D22接ENA
* D23接ENB
(3) 四顆馬達
* 左兩顆正極接OUT1
* 左兩顆負極接OUT2
* 右兩顆正極接OUT3
* 右兩顆負極接OUT4
## 5. 使用Dabble App連線
* 右上角藍牙連接裝置"HannahCar"
* 使用GamePad可開始遙控車子
