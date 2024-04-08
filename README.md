# KDDI
公開している成果物がある方は公開名称と公開URLは以下の通りです

a._成果物の内容_：

再構成行列の疎な特性を活用して再構築アルゴリズムを修正し、 既存の方法と比較して、再構築速度を数百倍に向上させました。

_作成に至った経緯_：



_使用言語_：verilog

1. **Jiayao Xu**, Pham Do Kim Chi, Chen Fu, Jinjia Zhou, "An 81.92 Gpixels/s Fast Reconstruction of Images from Compressively Sensed Measurements." 2022 IEEE International Symposium on Circuits and Systems **(ISCAS)**. IEEE, 2022.

   Link: https://ieeexplore.ieee.org/abstract/document/9937930?casa_token=Zpj9J10dxAEAAAAA:pQbQqBv1rEEM85xG1VeMAJVacjuYTercxw23pHZCJbF8sFquH7OpT3pxlDkqDddnwvDwouhFVw
2. **Jiayao Xu**, Chen Fu, Zhiqiang Zhang, Jinjia Zhou, "Real-time FPGA Design for OMP Targeting 8K image Reconstruction", The 28th International Conference on Multimedia Modeling **(MMM)**, 2022.

   Link: https://link.springer.com/chapter/10.1007/978-3-030-98358-1_41
   
b._成果物の内容_：

一部の再構築をencoderに移植し、より疎なデータを取得し、画質の劣化を低減しながら圧縮率を向上させます。既存の方法と比較して、私たちの方法ではエンコードおよびデコード時間を節約し、同時にビットあたりのピクセル数を減らしながら画像の品質を向上させました。

_作成に至った経緯_：

圧縮センシングを利用した画像codecの主要な課題は、時間コストと圧縮率です。既存の手法では、伝統的なcodecのencoding手法（例：intra-prediction）が導入され、圧縮率が向上していますが、時間コストが増加しています。以前の成果で改良された再構築方法の一部の処理後のデータが元のデータよりもより疎であることに気付きました。したがって、この一部をencoderに移動し、圧縮率を向上させると同時に、時間コストを大幅に低減しました。 

_使用言語_：matlab

3. **Jiayao Xu**, Jian Yang, Fuma Kimishima, Ittetsu Taniguchi, Jinjia Zhou. "Compressive Sensing Based Image Codec With Partial Pre-Calculation," in **IEEE Transactions on Multimedia**, doi: 10.1109/TMM.2023.3327534. **(IF=8.182)**

   Link: https://ieeexplore.ieee.org/abstract/document/10297548?casa_token=f9MV8znLGNQAAAAA:dhbiX_nx31i7HVsoQZ4y2gZE-dRi-0gdlMPdwHVmFGBOf3ztBWWhi-5x1K0oa1nPWJo3INj5HQ

c._成果物の内容_：既存の圧縮センシングフレームワークを変更することなく使用できる適応型サンプリング手法を設計し、同じ圧縮率の下でより高品質な再構築画像を得ることができました

_作成に至った経緯_：

_使用言語_：Python

4. **Jiayao Xu**, Jinjia Zhou. "Plug-and-Play Adaptive Block Compressive Sensing using Edge-Detection in the Compressed Domain" Computational Visual Media, **IF 6.9**. (Under Peer-reviewing).
