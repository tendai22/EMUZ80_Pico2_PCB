# EMUZ80_Pico2_PCB
KiCad PCB for emuz80_pico2

## WeAct RP2350B Core Board での動作

GPIO23を D7 に割り当てているが、D7 だけ L に落ちてくれない。

一瞬 L になるが、次の瞬間に H に戻っている。

blink で GPIO23 を指定したときは動作している。

Pimoroni 2350 の試作基板では動作している。

ハードウェアの違いによると考えられる。

基板の配線違いか、5.1kΩのプルアップが悪さをしていると考えた。

導通を見る限り怪しいところとつながっている様子はない。

結局 5.1kΩプルアップ抵抗をちぎり取って動作するようになった。なんとも。

<img src="img/001-RP2350-Core-Board-KEY-circuit-anno.png"/>
<img src="img/002-RP2350-Core-Board-remove-51kohm.png">