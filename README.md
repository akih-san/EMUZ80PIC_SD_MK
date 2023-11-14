# EMUZ80PIC_SD MK2.2, MK3.2
<br>
EMUZ80PIC_SDは、EMUZ80にアドオンするμSDカードモジュールです。<br>
今回、新たに2種類のμSDカードモジュールを作ってみました。<br>
<br>
<br>
![EMUZ80PIC_SD No.1](Photo/P3.jpg)<br>
![EMUZ80PIC_SD No.2](Photo/P4.jpg)
<br>
<br>
第一弾に比べて、LEDの数を増やしました。<br>
PICがバスを占有していることを示す/BUSRQの信号でＬチカします。<br>
/SPI_CSの信号と微妙に違うタイミングでLチカすることを楽しめます。(笑)<br>
とは言っても、SDカードアクセス時には両方ほぼ同時にLチカしますが(;'∀')<br>
<br>
<br>
今回公開するのは、ガーバーデータと図面、部品表となります。<br>
<br>
第一弾のEMUZ80PIC_SDは、以下を参照してください。ファームウェアもそこにあります。<br>
https://github.com/akih-san/EMUZ80PIC_SD<br>
<br>
<br>
このμSDカードモジュールは、EMUZ80+SuperMEZ80、または、EMUZ80+MEZZ180RAMの組み合わせで、<br>
CP/M-80 Ver2.2を走らせることが出来ます。<br>
<br>
EMUZ80は、電脳伝説(@vintagechips)さんによって作成された2チップで動作するシンプルなSBCです。<br>
SuperMEZ80、MEZZ180RAMは、@S_Okueさんによって作成されたEMUZ80用のメザニンボードです。<br>
<br>
EMUZ80、SuperMEZ80、MEZZ180RAMは、オレンジピコショップでお求めになれます。<br>
https://store.shopping.yahoo.co.jp/orangepicoshop/<br>
<br>
# EMUZ80PIC_SD MK2.2
秋月電子通商で販売されている、μSDカードスロットレベルシフタ付きブレークアウト基板キット<br>
(AE-microSD-LLCNV)を採用しています。2.54mm間隔のDIP用基板なので、ハンダ付けの作業も楽です。<br>
第一弾のμSDカードモジュールはμSDカードをコネクタで接続していましたが、MK2.2ではハンダ付け<br>
されるので、安定した固定感を得られます。<br>
作成上の注意点がありますので、「EMUZ80PIC_SD MK2.2作成上の注意点.pdf」を参照の後に作成を<br>
してください。<br>
<br>
<br>
![EMUZ80PIC_SD MK2.2 No.1](Photo/EMUZ80PIC_SD MK2.2.png)
![EMUZ80PIC_SD MK2.2 No.2](Photo/P1.jpg)
<br>
<br>
# EMUZ80PIC_SD MK3.2
<br>
EMUZ80PIC_SD MK3.2は、SMD部品を使い、μSDカードを基板に直接取り付ける事で、第一弾の<br>
EMUZ80PIC_SDと同じ面積に全ての部品を実装しています。<br>
一番コンパクトな仕上がりとなっています。<br>
ただし、チップ抵抗等は敢えて使わず、カラーコードの抵抗等を使用してレトロ感？を出してみました。<br>
カラー抵抗の色どりが、味わい深いと思います(^^♪<br>
<br>
ただし、SMDなだけに、ハンダ付けの難易度が上がります。HD74LVC541ATELLは0.65mmピッチなので<br>
リフロー出来る方は、リフローした方が確実です。<br>
ハンダに自身の無い方は、EMUZ80PIC_SD MK2.2を選択した方が無難かと思います。<br>
<br>
<br>
![EMUZ80PIC_SD MK3.2 No.1](Photo/EMUZ80PIC_SD MK3.2.png)
![EMUZ80PIC_SD MK3.2 No.2](Photo/P2.jpg)
<br>
<br>
＜参考＞<br>
・EMUZ80<br>
EUMZ80はZ80CPUとPIC18F47Q43のDIP40ピンIC2つで構成されるシンプルなコンピュータです。<br>
<br>
＜電脳伝説 - EMUZ80が完成＞  <br>
https://vintagechips.wordpress.com/2022/03/05/emuz80_reference  <br>
＜EMUZ80専用プリント基板 - オレンジピコショップ＞  <br>
https://store.shopping.yahoo.co.jp/orangepicoshop/pico-a-051.html<br>
<br>
・SuperMEZ80<br>
SuperMEZ80は、EMUZ80にSRAMを追加し、Z80をノーウェイトで動かすことができるメザニンボードです<br>
<br>
SuperMEZ80<br>
https://github.com/satoshiokue/MEZ80RAM<br>
https://github.com/satoshiokue/SuperMEZ80<br>
<br>
・MEZZ180RAM<br>
MEZZ180RAMは、EMUZ80にZ180+SRAMのメザニンボードです。HD64180R/ZやZ8S180が動作します。<br>
<br>
MEZZ180RAM<br>
https://github.com/satoshiokue/MEZZ180RAM<br>
https://github.com/satoshiokue/EMUZ80-Z180RAM<br>
