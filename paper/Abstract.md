# Abstract

リカレントバックプロパゲーションを使用して長い時間間隔にわたって情報を保存することを学習するのは非常に時間がかかります。これは主に、不十分で減衰する誤差逆伝播が原因です。

この問題に関するHochreiterの1991年の分析を簡単にレビューし、その後、新しい効率的な勾配ベースの手法「Long Short-Term Memory」（LSTM）を導入して対処します。

勾配を無害な範囲で切り捨てることで、LSTMは特別なユニット内の「Constant Error Carrousels（CEC）」を介してconstant error flowを強制し、1000を超える離散時間ステップの最小タイムラグを橋渡しすることを学習できます。

Multipulgate unitは、constant error flowへのアクセスを開閉することを学習します。

LSTMは空間と時間において局所的であり、時間ステップおよび重みあたりの計算複雑度は𝑂(1)です。

我々の人工データに関する実験は、局所的、分散的、実数値、ノイズのあるパターン表現を含みます。

RTRL、BPTT、Recurrent Cascade-Correlation、Elmanネット、およびNeural Sequence Chunkingとの比較では、LSTMはより多くの成功した試行をもたらし、はるかに速く学習します。

LSTMはまた、以前のリカレントネットワークアルゴリズムでは解決できなかった複雑な人工の長いタイムラグタスクも解決します。
