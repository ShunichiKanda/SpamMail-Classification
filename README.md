# SpamMail-Classification
ProbSpaceの「スパムメール判別」コンペに挑戦した。
https://prob.space/competitions/spam_mail
## EDA

訓練データは、非スパム:スパム = 8707件:171件であり、不均衡データが特徴である。
そのため、異常検知としてモデル構築する必要がある。

不均衡データへの対処策としては、
- Undersampling
- Oversampling (自然言語処理であるため工夫が必要である)
- 損失関数の重みを変える
等が考えられる。

なお、テストデータは、非スパム:スパム = 7838件:17000件と比率が逆転しており、注意が必要である。