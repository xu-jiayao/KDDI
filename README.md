# Publication and code (日本語)
公開している成果物がある方は公開名称と公開URLは以下通りです。

## 1
### 成果物の内容：

再構成行列の疎な特性を活用して再構成アルゴリズムを修正し、既存の方法と比較して、再構成速度を数百倍に向上させました。

### 作成に至った経緯：

再構成速度は、圧縮センシングのアプリケーションにおける主要な問題の一つです。速度の問題に対処するため、多くの研究はアルゴリズムをハードウェア上で実装することを選択しています。しかし、大量の逆行列計算とベクトル積は、ハードウェア実装と速度向上の2つの主要な障害となっています。これらの2つのボトルネックを克服するために、私たちの研究では、再構成に疎な性質を持つ行列を選択し、行列の疎な性質を活用して再構成を適化し、8Kのリアルタイム再構成を実現しました。

### 使用言語：Verilog

1. **Jiayao Xu**, Pham Do Kim Chi, Chen Fu, Jinjia Zhou, "An 81.92 Gpixels/s Fast Reconstruction of Images from Compressively Sensed Measurements." 2022 IEEE International Symposium on Circuits and Systems **(ISCAS)**. IEEE, 2022.

   Paper Link: https://ieeexplore.ieee.org/abstract/document/9937930?casa_token=Zpj9J10dxAEAAAAA:pQbQqBv1rEEM85xG1VeMAJVacjuYTercxw23pHZCJbF8sFquH7OpT3pxlDkqDddnwvDwouhFVw

   Code Link: https://drive.google.com/drive/folders/1_ShwuAg9EZso5yeUg97F6ysxes0qgwW9?usp=drive_link
3. **Jiayao Xu**, Chen Fu, Zhiqiang Zhang, Jinjia Zhou, "Real-time FPGA Design for OMP Targeting 8K image Reconstruction", The 28th International Conference on Multimedia Modeling **(MMM)**, 2022.

   Paper Link: https://link.springer.com/chapter/10.1007/978-3-030-98358-1_41

   Code Link: https://drive.google.com/drive/folders/1W4ylhluBqIZIAeQLW02U7Uw7cjY3Azq9?usp=sharing

   
## 2

### 成果物の内容：

一部の再構成をエンコーダに移植することで、より疎なデータを取得し、画質の劣化を低減しながら圧縮率を向上させます。この方法では処理時間を節約し、同時にbppを減らしながら画像の品質を向上させました。

### 作成に至った経緯：

圧縮センシングを利用した画像コーデックの主要な課題は、時間コストと圧縮率です。既存の手法では、伝統的なコーデックのエンコード手法（例：イントラ予測）が導入され、圧縮率が向上していますが、時間コストが増加しています。以前の成果で改良された再構築方法の一部の処理後のデータが、元のデータよりもさらに疎であることに気付きました。したがって、この一部をエンコーダに移動させることによって、圧縮率を向上させると同時に、時間コストを大幅に低減しました。

### 使用言語：MATLAB

3. **Jiayao Xu**, Jian Yang, Fuma Kimishima, Ittetsu Taniguchi, Jinjia Zhou. "Compressive Sensing Based Image Codec With Partial Pre-Calculation," in **IEEE Transactions on Multimedia**, doi: 10.1109/TMM.2023.3327534. **(IF=8.182)**

   Paper Link: https://ieeexplore.ieee.org/abstract/document/10297548?casa_token=f9MV8znLGNQAAAAA:dhbiX_nx31i7HVsoQZ4y2gZE-dRi-0gdlMPdwHVmFGBOf3ztBWWhi-5x1K0oa1nPWJo3INj5HQ

   Code Link: https://drive.google.com/drive/folders/18kKib23EpEU7K-PZPoSYVM0M7tc2W6kV?usp=sharing

## 3

### 成果物の内容：

既存の圧縮センシングフレームワークを変更せずに、使用可能な適応型サンプリング手法を設計し、同じ圧縮率の下でより高品質な再構成画像を得ることができました。
　
### 作成に至った経緯：

圧縮センシングのほとんどの研究では、均一サンプリングが採用されており、つまり、ブロック内の情報量にかかわらず、一定のサンプリングレートが採用されています。この手法は、情報量が多いブロックの画質を劣化させます。この問題を解決するため、既存の手法では適応型サンプリングが採用され、画像ブロックの情報量を計算します。その情報量に基づいてサンプリングレートが割り当てられます。しかし、これらの手法は2回のサンプリングと再構成が必要であり、時間とハードウェアコストが大幅に増加しています。私たちは、適応型サンプリング方法を提案し、サンプリングされたデータを使用して画像ブロックの情報量を判断し、これに基づいてサンプリングレートを割り当てます。この方法は、既存の圧縮センシングのフレームワークを変更する必要がなく、プラグアンドプレイを実現し、1回のサンプリングと再構成のみで済みます。これにより、適応型サンプリングフレームワークの時間とハードウェアコストが大幅に節約されます。

### 使用言語：Python, MATLAB

4. **Jiayao Xu**, Jinjia Zhou. "Plug-and-Play Adaptive Block Compressive Sensing using Edge-Detection in the Compressed Domain" Computational Visual Media, **IF 6.9**. (Under Peer-reviewing).

   Code Link: https://drive.google.com/drive/folders/17O8s4Ljr-9btgemcEsap7fnzLaWKEH7b?usp=sharing
   
## 4

### 成果物の内容：

iSWUSTは、モバイルWeb研究室によって開発されたキャンパス内の学生向けのアプリです。このアプリでは、講義スケジュールや図書館の本などの情報収集、そしてキャンパスカードの残高確認やチャージのサービスなど、3,000人以上のユーザーにサポートを提供していました。

### 作成に至った経緯：

1. APIの設計に参加し、APIドキュメントを変更して、開発チームに理解させ、効果的に使用させるようになりました。

2. 既存のアプリケーションをリファクタリングし、Gitバージョン管理を活用してコードの共同作業とプロジェクト管理を効率化しました。異なるデザインパターンを活用して結合度を最小限に抑え、コードの保守性を向上させました。

3. ライブラリとログインモジュールの機能を設計および実装し、コードの正確性を検証し、システムの安定性を強化するためのテスト手法を組み込みました。

4. ネットワークレイヤーを実装し、データパケットのJSONカプセル化を行いました。バックエンドチームと協力してネットワークレイヤーをテストし、バックエンドサービスとのシームレスな通信を確保し、要件を満たすために必要な調整を行いました。

### 使用言語：Objective-C

アプリが既にストアから削除されていますので、現時点では私が担当しているコードのみが公開可能です。

Code Link: https://drive.google.com/drive/folders/18b4DR9fAv26g04fVfTeM9fF_aYwpOp6E?usp=sharing

