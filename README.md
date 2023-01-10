# Final-project
### 資工二 110321056 陳冠仲 
### 資工二 110321027 張啟廣
## 語言環境
Verilog \
Quartus 13.1
## 照片
  ![game](https://user-images.githubusercontent.com/122383629/211610812-e33b9299-2bb5-463a-83ac-d4cdb30b7008.jpg)
## 功能說明
a. 七段顯示器顯示累計得分數 \n
b. LED燈顯示血條 \n
c. 黃色障礙物來阻擋球 \n
d. 每打到磚塊得一分 \n
e. 除原本的球之外，會偶爾出現特殊球(粉紅球)無視障礙物直接打到磚塊 \n
f. 可手動調整球速 \n
g. 勝利時會顯示WIN，輸了會顯示LOSE \n
h. 打到磚塊會發出聲音 \n
## 程式 input/output 說明
module final( \n
	input CLK, reset, start, \n
	output reg [0:27] led, \n
	output reg [4:0] life, \n
	input left, right, \n
	input throw, \n
	input show_two_row, \n
	output testLED,\n
	output reg a,b,c,d,e,f,g,\n
	output reg [0:3] COM,\n
	input highSpeed,\n
	output reg beep\n
);\n
