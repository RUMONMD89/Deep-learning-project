# Deep-learning-project
(**cats-vs-dogs-classification**)

## CNN を使用した猫と犬の分類

畳み込みニューラル ネットワーク (CNN) は、畳み込み層を適用することによって動作し、conv2d などの演算を利用して学習したフィルター (カーネル) を入力画像と畳み込みます。 これらのフィルターは、画像のさまざまな側面に重みとバイアスを割り当て、特徴抽出を支援します。
バッチ正規化を適用して、バッチ全体で入力を正規化することで学習を強化します。 
 ネットワーク パラメーターは、予測とラベルの間の距離を最小化するために反復的に調整されます。 このプロセスはバッチごとに繰り返され、ネットワークの予測機能が徐々に向上します。...
 バッチ正規化する前の結果として
 
<img src="old_val_accuracy.png" height="400px" width ="550px">　
<img src="old loss_accuracy.png" height="400px" width ="550px">　

学習を強化し予測機能が徐々に向上するため いくつか方法があります。

データの追加
データ拡張
L1/L2 正規化 (古い手法)
ドロップアウト
バッチ正規化
複雑さの軽減

「ドロップアウトとバッチノルム」技術を適用して過剰適合を減らします。

<img src="new val_accuracy.png" height="400px" width ="550px">　
<img src="new loss_accuracy.png" height="400px" width ="550px">　
