# USB-C_PCB_Receptacle

プリント基板でできたUSB Type-Cコネクタです。

## 概要
- プリント基板製 USB Type-C リセプタクル
- シェル部分が無いためケーブルに負荷がかかりやすく破損の恐れがあります。試験用、実験用としてご使用ください。

## 外観
![基板全体](/images/pcb-sheet.jpg)
![子基板表面裏面](/images/pcb-piece.jpg)

## スペック
- シート(集合基板)サイズ：97.28 x 91.28
- ピース(子基板)サイズ：10.16 x 12.7
- 48ピース/1シート
- 基板厚：0.8mm (製造可否は各プリント基板メーカーにお問い合わせください。)
- 信号線：VBUS, GND, CC1, CC2, D+, D-

## KiCad設計データ
- [回路図 (ブラウザで見る)](https://kicanvas.org/?github=https%3A%2F%2Fgithub.com%2Fsuzan-works%2FUSB-C_PCB_Receptacle%2Fblob%2Fmain%2Fkicad%2FUSB-C_PCB_Receptacle.kicad_sch)
- [回路図 (PDF)](/kicad/USB-C_PCB_Receptacle.pdf)
- [基板設計データ (ブラウザで見る)](https://kicanvas.org/?github=https%3A%2F%2Fgithub.com%2Fsuzan-works%2FUSB-C_PCB_Receptacle%2Fblob%2Fmain%2Fkicad%2FUSB-C_PCB_Receptacle.kicad_pcb)

## 使用例
- ブレッドボードやユニバーサル基板で、気軽にUSB-Cコネクタが使えます。
- 抵抗5.1kΩを2個実装することで、USB PD 対応電源から簡単に5Vが得られます。
(プルダウン抵抗5.1kΩをCC1, CC2に実装することで、USB PD仕様に基づいた5V供給を要求する信号が生成され、対応する電源から5Vが供給されます。)

![使用例1](/images/usage-example-1.jpg)
![使用例2](/images/usage-example-2.jpg)
![使用例3](/images/usage-example-3.jpg)

## 参考
- [CH552E Breakout - CH552Eブレークアウト](https://www.switch-science.com/products/8911) : USB Type-Cエッジコネクタを備えておりケーブルに直接接続可能なマイコンボード。WCH社製8ビットUSBマイコンCH552Eを搭載。
- [Carduino クレジットカードサイズのフィジカルコンピュータ](https://bit-trade-one.co.jp/adakcadu/) : USB Type-Cコネクタ搭載でケーブル接続可能なマイコンボード。クレジットカードサイズのArduino UNO互換機。
- [Carduino USB-C_PCBPLUG](https://github.com/akita11/Carduino/blob/master/Carduino_v41.pretty/USB-C_PCBPLUG.kicad_mod) : CarduinoのUSB Type-CコネクタのKiCadライブラリ。
- [USB Implementers Forum 公式資料](https://www.usb.org/documents)  
　"USB Type-C Cable and Connector Specification Release 2.4" > "Figure 3-1 USB Type-C Receptacle Interface Dimensions"

## ライセンス
[MIT License](https://opensource.org/licenses/MIT)
