# Deep-learning-project
(**cats-vs-dogs-classification**)

## CNN を使用した猫と犬の分類

畳み込みニューラルネットワーク（CNN）は、畳み込み層を通じて学習済みのフィルター（カーネル）を用い、入力画像から特徴を抽出します。このフィルターは、画像の様々な側面に重みとバイアスを適用し、特徴抽出を助けます。さらに、バッチ正規化を用いてバッチ全体で入力を正規化することで、学習を安定化させ、効率を高めます。ネットワークは、予測とラベルの間の誤差を最小化するためにパラメーターを反復的に調整し、バッチごとにその予測精度が向上していきます。バッチ正規化を導入する前には、学習が不安定になりやすいことが観察されます。
 バッチ正規化する前の結果として-----
 
<img src="old_val_accuracy.png" height="400px" width ="550px">　
<img src="old loss_accuracy.png" height="400px" width ="550px">　

学習を強化し予測機能が徐々に向上するため いくつか方法があります。


1) データの追加
2) データ拡張
3) L1/L2 正規化 (古い手法)
4) ドロップアウト
5) バッチ正規化
6) 複雑さの軽減

今回「ドロップアウトとバッチ正規化」技術を適用して過剰適合(data overfitting)を減らします。

<img src="new val_accuracy.png" height="400px" width ="550px">　
<img src="new loss_accuracy.png" height="400px" width ="550px">　

「ドロップアウトとバッチ正規化」を適用することで、学習プロセスが強化され、訓練データとテストデータ間の性能差（ギャップ）を埋める効果が得られます。これにより、モデルの過学習が抑えられ、汎化性能が向上して、全体的な正確性が増す結果が期待できます。
