# LLMs

## The History of Chatbots

```mermaid
flowchart

ELIZA --> Chatbot --> 人工無能 --> Siri --> ChatGPT

```

*[ELIZA](https://en.wikipedia.org/wiki/ELIZA) (1966)*
初期の人工知能プログラムのひとつ。
ルールベースの簡単なパターンマッチングで返答していた。
ELIZA(DOCTOR)は心理療法士の会話を模したものが有名。

*[PARRY](https://ja.wikipedia.org/wiki/PARRY) (1972)*
PARRYは偏執病的統合失調症患者をシミュレートしようとしたもの。
ELIZA(DOCTOR)と通信し話題となった。

*[A.L.I.C.E.](https://ja.wikipedia.org/wiki/Artificial_Linguistic_Internet_Computer_Entity) (1995)*
ヒューリスティックパターンマッチングを使用している。
AIML(Artificial Intelligence Markup Language)というXMLベースで条件を記述できた。
AIMLはGPLライセンスで公開されたため、後の多くのチャットボットがGPLで作成されることとなった。
ローブナー賞(Loebner Prize)というチャットボットが人間と区別できないほどの会話能力を持つか評価するコンテストで優勝して話題となった。
ローブナー賞を2000年、2001年、2004年に受賞している。

*[Jabberwacky](https://ja.wikipedia.org/wiki/Jabberwacky) (1997)*
ユーモラスな人間同士の自然な会話をシミュレートすることを目的としていた。
ユーザーとの会話の大規模なデータベースを構築し、言語と文脈を学習することができた。
ローブナー賞を2003年、2005年、2006年に受賞している。

*[人工無能](https://ja.wikipedia.org/wiki/%E4%BA%BA%E5%B7%A5%E7%84%A1%E8%84%B3) (1995)*
一方日本では、ゆいぼっとや人工無能うずらが流行っていた。
日本語は分かち書きされておらず、[形態素解析](https://ja.wikipedia.org/wiki/%E5%BD%A2%E6%85%8B%E7%B4%A0%E8%A7%A3%E6%9E%90)などの前処理が必要だった。

代表的な形態素解析ソフトウェアは以下の通り。
[JUMAN](https://ja.wikipedia.org/wiki/JUMAN) (1987)
[ChaSen 茶筌](https://ja.wikipedia.org/wiki/ChaSen) (1995)
[MeCab 和布蕪](https://ja.wikipedia.org/wiki/MeCab) (2005)
JUMAN++ (2015)

*[デスクトップ マスコット](https://ja.wikipedia.org/wiki/%E4%BC%BA%E3%81%8B) (1998)*
その後、ペルソナウェア、偽ペルソナウェア、伺か、が流行っていた。

*[IBM Watson](https://en.wikipedia.org/wiki/IBM_Watson) (2011)*
クイズ番組に出場させるために開発された。

2013年には、Watsonにより人間味を持たせようと俗語辞書Urban Dictionaryを学習させたことにより、下品な言葉遣いになった事例がある。
この試みは中断され、スマートフィルターが開発されることとなった。

*[Siri](https://ja.wikipedia.org/wiki/Siri) (2011)*
Hey, Siri!
iPhoneに搭載され話題となった。

*[Google Now](https://ja.wikipedia.org/wiki/Google_Now) (2012)*
OK, Google!
Androidに搭載され話題となった。

*[Mitsuku](https://en.wikipedia.org/wiki/Kuki_AI) (2013)*
A.L.I.C.E.で開発されたAIMLを基にしている。
2013年から2019年の間にローブナー賞を5回受賞している。
これ以降はローブナー賞は中止された。

2021年にはKuki AIという名前に代わり、メタバースに進出した。

*[Alexa](https://ja.wikipedia.org/wiki/Amazon_Alexa) (2014)*
Amazon Echoに搭載され話題となった。
スキルと呼ばれるサードパーティ製のアプリを活用することができる。
同時期にWindowsのCortanaなどがある。

*[りんな](https://ja.wikipedia.org/wiki/%E3%82%8A%E3%82%93%E3%81%AA_(%E4%BA%BA%E5%B7%A5%E7%9F%A5%E8%83%BD)) (2015)*
女子高生AIとしてLINEに登場して話題となった。

同時期にMicrosoft Tayが登場しているが、ユーザーとの会話を学習する機能により調教されたため、問題発言を繰り返し終了された。

*[Googleアシスタント](https://ja.wikipedia.org/wiki/Google_%E3%82%A2%E3%82%B7%E3%82%B9%E3%82%BF%E3%83%B3%E3%83%88) (2017)*
双方向の会話が可能となった。
今までのGoogle Nowの仕組みと組み合わせて、音声でAndroidを操作することができる。

*[Meena](https://ja.wikipedia.org/wiki/LaMDA) (2020)*
人間に近いオープンドメインのチャットボットとして公開された。
感性を持って応答するように訓練されている。

*[ChatGPT](https://ja.wikipedia.org/wiki/ChatGPT) (2022)*
OpenAIが開発した大規模言語モデルGPT-3.5を利用したシステム。
大規模言語モデルの特徴として、対話だけでなく、要約や翻訳などさまざまな自然言語処理を行うことができる。
Codexなどを組み込み爆発的な人気を呼んだ。

## The History of LLMs

```mermaid
flowchart

RNN --> LSTM --> Word2Vec --> GloVe
Word2Vec --> fastText
LSTM --> Seq2Seq --> Attention
RNN --> GRU
```

*[RNN](https://ja.wikipedia.org/wiki/%E5%9B%9E%E5%B8%B0%E5%9E%8B%E3%83%8B%E3%83%A5%E3%83%BC%E3%83%A9%E3%83%AB%E3%83%8D%E3%83%83%E3%83%88%E3%83%AF%E3%83%BC%E3%82%AF) (1986, 2012)*
RNNの考え自体は昔からあった。
中間層で再帰的な結合があり、時系列のデータを処理することができた。
しかし、再帰的な処理は計算コストが高く、ハードウェアの性能が足りなかった。
また勾配消失があり学習が収束しない問題があった。
そのため、RNN以外の研究に移っていった。

CNNでDeep Learningが注目を集め、RNNにも注目が戻ってきた。

*[LSTM](https://ja.wikipedia.org/wiki/%E9%95%B7%E3%83%BB%E7%9F%AD%E6%9C%9F%E8%A8%98%E6%86%B6) (1997, 2007)*
RNNの勾配消失を解決するためにLSTMが登場した。
長期的な記憶を保持することができるようになった。
しかし、実際には、非常に長い依存関係を適切にとらえることは難しかった。

*[GRU](https://ja.wikipedia.org/wiki/%E3%82%B2%E3%83%BC%E3%83%88%E4%BB%98%E3%81%8D%E5%9B%9E%E5%B8%B0%E5%9E%8B%E3%83%A6%E3%83%8B%E3%83%83%E3%83%88) (2014)*
LSTMよりも簡単な構造を持ち、パラメータ数が少なく、計算コストが低い。
いくつかの問題ではLSTMに類似する性能が発揮された。
しかし、LSTMの優位性を上回ることができなかった。

*[Word2Vec](https://ja.wikipedia.org/wiki/Word2vec) (2013 Google)*
Word2Vecというワードをベクトル化して計算できる手法が登場した。

*[GloVe](https://en.wikipedia.org/wiki/GloVe) (2014.01.02 Stanford)*
[Global Vectors for Word Representation](https://aclanthology.org/D14-1162/)
Word2Vecの局所的(local)な表現と、大局的(Global)な表現を組み合わせた手法。

*[fastText](https://en.wikipedia.org/wiki/FastText) (2015 Facebook)*
[facebookresearch/fastText](https://github.com/facebookresearch/fastText)
Self-Attentionの原型。

*[Seq2Seq](https://en.wikipedia.org/wiki/Seq2seq) (2014 Google)*
EncoderとDecoderを搭載したSeq2Seqという手法が登場した。
Seq2Seqは、翻訳や対話システム、要約などの様々な自然言語処理のタスクで、高い精度を達成することができた。

*[Attention](https://ja.wikipedia.org/wiki/%E3%82%A2%E3%83%86%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%B3_(%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92)) (2015.09)*
[Effective Approaches to Attention-based Neural Machine Translation](https://arxiv.org/abs/1508.04025)
ニューラル機械翻訳において、従来のSeq2SeqにAttentionメカニズムを導入することで、翻訳の品質を向上させることができた。

```mermaid
flowchart

Attention --> Transformer
LSTM --> ELMo
LSTM --> ULMFiT
Transformer --> Sparse-Transformer
Transformer --> Reformer

```

*[Transformer](https://ja.wikipedia.org/wiki/Transformer_(%E6%A9%9F%E6%A2%B0%E5%AD%A6%E7%BF%92%E3%83%A2%E3%83%87%E3%83%AB)) (2017.06.12 Google)*
[Attention Is All You Need](https://arxiv.org/abs/1706.03762)
RNNやLSTMは再帰的に処理を行うため、長い文脈だと計算コストが増大する問題があった。
Scaled Dot-Product Attentionを用いることで、長期依存関係を効率的に処理できるようになった。
またAttentionを複数のヘッドで並列にするMulti-Head Attentionの形態を取る。
RNNとは違い、全ての位置の計算を同時に行うことが可能となり、GPUを効率的に使用できるようになった。

Scaled Dot-Product AttentionはSelf-Attentionの一種で、必要なメモリが文章の長さの二乗に比例する。
LSTMに比べて計算速度は速いが、入力が長くなると計算負荷が高い。

*[ELMo](https://en.wikipedia.org/wiki/ELMo) (2018.02.15 AllenAI)*
パラメータ数: 300M
Word2VecやGloVeでは単語のみのベクトル化だったので、文脈を考慮できるようにしたもの。
2層のLSTMを2つ使った、双方向LSTM。

*ULMFiT (2018.02.18 fast.ai)*
[Universal Language Model Fine-tuning for Text Classification](https://arxiv.org/abs/1801.06146)
事前学習(Pre-train)と微調整(Fine-tuning)という今のLLMの原型となるもの。

*Sparse Transformer (2019.04.23 OpenAI)*
[Generating Long Sequences with Sparse Transformers](https://arxiv.org/abs/1904.10509)
通常のTransformerでは、トークンが他の全てのトークンと相互作用する全結合となっているが、
Sparse Transformerでは、一部のトークンのみと相互作用する手法を用いてメモリ効率を改善している。
通常のTransformerが $O(n^2)$ に対し、Sparse Transformerは $O(n\sqrt{n})$ となる。

*Reformer (2020.01.16 Google)*
[Reformer: The Efficient Transformer](https://arxiv.org/abs/2001.04451)
Transformerと比べ大幅にメモリ効率を改善した手法。
通常のTransformerが $O(n^2)$ に対し、Reformerは $O(n\log{n})$ となる。
RevNetとLSHという仕組みを用いている。

RevNet(Reversible Residual Network)とは、
ニューラルネットワークの各層の入力を保存する代わりに、前の層の入力を再計算することでメモリ使用量を減らす手法。

LSH(Locality-Sensitive Hashing)とは、
ベクトルの近似的な最近傍を効率的に検索するための手法。

```mermaid
flowchart

Transformer --> GPT --> GPT-2 --> GPT-3
GPT-3 --> InstructGPT --> ChatGPT
GPT-3 --> Codex --> ChatGPT
GPT-3 --> GPT-3.5 --> ChatGPT
GPT-3.5 --> GPT-4
```

*[GPT](https://ja.wikipedia.org/wiki/GPT_(%E8%A8%80%E8%AA%9E%E3%83%A2%E3%83%87%E3%83%AB)) (2018.06.11 [OpenAI](https://ja.wikipedia.org/wiki/OpenAI))*
パラメータ数: 110M(12層)
GPTの初期モデル。
TransformerのDecoderを用いて、大規模テキストデータで学習したものがGPTとなる。
Transformerが12層連なっているためモデルが大きい。

ELMoのLSTMが特徴抽出が十分でなかったため、Transformerを使用する手法が考えられた。
しかし、双方向ではなくなり、後のBERTの登場につながった。
一方向から推測するので、BERTよりテキスト生成タスクに向いている。

BookCorpus 7000冊のデータ4.5GB を事前学習に用いた。

*[GPT-2](https://ja.wikipedia.org/wiki/GPT-2) (2019.02.14 OpenAI)*
パラメータ数: 1.5B(48層)
人間が読んでも違和感が少ない一貫した内容の文章を生成できるようになった。

WEBから収集した40GBのデータで学習した。

*[GPT-3](https://ja.wikipedia.org/wiki/GPT-3) (2020.05.28 OpenAI)*
パラメータ数: 175B(96層)
GPT-3を超えたあたりでとても優秀になった。
OpenAIはGPT-3はClosed-Sourceとした。

WEBから収集した570GBのデータで学習した。
約100万ドルかかったと報告されている。

[Scaling Laws for Neural Language Models](https://arxiv.org/abs/2001.08361)
OpenAIはTransformerの仕組みはスケーリング則に則り、大規模化が可能との論文を発表した。
パラメータ数N、データセットサイズD、計算予算Cの3つの変数のべき乗則に従う。

[Are Emergent Abilities of Large Language Models a Mirage?](https://arxiv.org/abs/2304.15004)
飛躍的にスコアが上がり、創発が起こったと話題となった。
しかし、単にスコア用のテストがある一定以上の水準がないといけないという研究結果が出ている。

*InstructGPT (2021.01 OpenAI)*
パラメータ数: 1.3B
[Training language models to follow instructions with human feedback](https://arxiv.org/abs/2203.02155)
GPT-3の小型版を使用して、RLHFを取り入れたモデル。
GPT-3よりも人間の指示に従う能力が優れている。

[RLHF](https://en.wikipedia.org/wiki/Reinforcement_learning_from_human_feedback)
RLHF(Reinforcement Learning from Human Feedback)は、
人間からのフィードバックでファインチューニングする手法。

*[OpenAI Codex](https://ja.wikipedia.org/wiki/OpenAI_Codex) (2021.08 OpenAI)*
[Evaluating Large Language Models Trained on Code](https://arxiv.org/abs/2107.03374)
自然言語からプログラムのソースコードを生成するためのモデル。
GPT-3をプログラミングのソースコードで微調整したもの。

GitHub Copilotを動かしていた初期モデル
code-cushman-001

*GPT-3.5 (2022.03.15 OpenAI)*
初期バージョン
text-davinci-002
code-davinci-002

*GPT-3.5v2 (2022.11.28 OpenAI)*
改良バージョン
gpt-3.5-turbo 会話用
text-davinci-003

*[ChatGPT](https://ja.wikipedia.org/wiki/ChatGPT) (2022.11.30 OpenAI)*
InstructGPTの兄弟モデル。
チャット向けに調整されている。

APIは従量課金制。
Azure OpenAI Serviceからも同じモデルのAPIを使用することができる。
なお、価格は同じで、レスポンスはAzureの方が早い模様。

*[GPT-4](https://ja.wikipedia.org/wiki/GPT-4) (2023.03.14 OpenAI)*
パラメータ数: 非公表
マルチモーダル。
システムメッセージという仕組みを導入した。
司法試験や大学入試試験(SAT)で受験者の上位10%に入る成績を出して話題となった。

1億ドル以上かかったとされる。

[GPT-4 Technical Report](https://arxiv.org/abs/2303.08774)
モデル規模を拡大することで得られる効果は逓減すると発表された。

```mermaid
flowchart

GPT-2 --> GPT-Neo --> GPT-NeoX
GPT-2 --> GPT-J
GPT-2 --> Pythia
```

*GPT-Neo (2021.03 [EleutherAI](https://en.wikipedia.org/wiki/EleutherAI))*
パラメータ数: 125M, 1.3B, 2.7B
GPT-3がClosed-Sourceだったので、Open-SourceのGPT-3を作成することを目的としたモデル。
GPT-2のクローンを作ろうとしたものをもとにしている。
256トークンのウィンドウサイズに区切ったLocal Attentionを使用している。
Local Attentionはウィンドウ外へアクセスできないため、パフォーマンスとのトレードオフとなる。

The Pileデータセットで訓練された。

*[GPT-J](https://en.wikipedia.org/wiki/GPT-J) (2021.05 EleutherAI)*
パラメータ数: 6B
JAXライブラリを使用していたのでGPT-Jと名づけられた。
公開された当時は、GPT-3スタイルのモデルとして世界最大のものだった。

Common Crawlデータセットで訓練された。

*GPT-NeoX (2022.02 EleutherAI)*
パラメータ数: 20B(44層)
EleutherAIが公開したLLM学習用のライブラリ、およびそれを用いてトレーニングされたモデル。
Microsoft DeepSpeedを使って学習を高速化している。
Nvidia Megatronを使って分散して学習した。
公開された当時は、GPT-3スタイルのモデルとして世界最大のものだった。

*Pythia (2023.02.13 EleutherAI)*
パラメータ数: 70M-12B および各モデルの154のチェックポイント
[Pythia: A Suite for Analyzing Large Language Models Across Training and Scaling](https://arxiv.org/abs/2304.01373)
[EleutherAI/pythia](https://github.com/EleutherAI/pythia)

LLMの訓練とスケーリングを分析するために作成されたため、多数のチェックポイントを残している。

```mermaid
flowchart

Transformer --> BERT
ELMo --> BERT --> RoBERTa --> LUKE
BERT --> DistilBERT
BERT --> ALBERT
BERT --> ELECTRA
BERT --> DeBERTa
```

*[BERT](https://ja.wikipedia.org/wiki/BERT_(%E8%A8%80%E8%AA%9E%E3%83%A2%E3%83%87%E3%83%AB)) (2018.10.11 Google)*
パラメータ数: BERT-base=110M, BERT-large=340M
[BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/abs/1810.04805)
GPTとは違い、TransformerのEncoderを使用し、文章の先頭と末尾からの双方向(Bidirectional)なAttention層が追加されている。
MLM(Masked Language Modeling)という手法を用いて、ラベリングなしの少ないデータから学習できた。
また文脈を予測するためにNSP(Next Sentence Prediction)という手法が用いられた。

GPT-1を超えて最高スコアを更新し、応用も効くため話題となった。
その後GPT-3が発表されるまでBERT系が多く登場することとなった。

*[RoBERTa](https://ai.facebook.com/blog/roberta-an-optimized-method-for-pretraining-self-supervised-nlp-systems/) (2019.07.26 Facebook)*
パラメータ数: RoBERTa-base=123M, RoBERTa-large=354M
[RoBERTa: A Robustly Optimized BERT Pretraining Approach](https://arxiv.org/abs/1907.11692)
BERTの仕組みをそのままに、パラメータの調整やデータ量を増大させたもの。

*DistilBERT (2019.08.02 [Hugging Face](https://ja.wikipedia.org/wiki/Hugging_Face))*
パラメータ数: 66M
BERTを蒸留したもの。
蒸留とは、大規模な教師モデルから小規模な生徒モデルを作成する手法。
DistilBERTはオリジナルのBERTと比べ約40%のパラメータを削減でき、性能を維持しつつ高速に動作するようになった。
しかし、蒸留の過程で情報が失われるため、より精度の高いものを求める場合はオリジナルが適している。

*[ALBERT](https://medium.com/syncedreview/googles-albert-is-a-leaner-bert-achieves-sota-on-3-nlp-benchmarks-f64466dd583) (2019.09.20 Google)*
パラメータ数: ALBERT-base=12M, ALBERT-large=18M, ALBERT-xlarge=60M, ALBERT-xxlarge=235M, ALBERT-xxlarge v2=233M
[ALBERT: A Lite BERT for Self-supervised Learning of Language Representations](https://arxiv.org/abs/1909.11942)
パラメータの因数分解と冗長性を排除することで、軽量化したモデル。

BERT-baseモデルを軽量化すると、12MパラメータのALBERT-baseモデルが作成できた。
これは89%の削減となるが、性能の低下はわずかだった。
モデルサイズが縮小されたので、より大規模な構成を行えるようになった。
ALBERT-xxlarge構成では最新のスコアを更新した。

*ELECTRA (20219.09.26 Stanford, Google)*
パラメータ数: ELECTRA-small=14M, ELECTRA-base=110M, ELECTRA-large=335M
[ELECTRA: Pre-training Text Encoders as Discriminators Rather Than Generators](https://arxiv.org/abs/2003.10555)
GANの手法を取り入れて、BERTの事前学習手法を改良した。
MLMは文章中のマスクした15%を学習できない問題点があった。
ELECTRAではReplaced Token Detectionという手法を用いて、より少ないデータで効率的な事前学習ができる。
RoBERTaの1/4の学習量で同等の精度を達成した。

*[DeBERTa](https://github.com/microsoft/DeBERTa) (2020.06.13 Microsoft)*
パラメータ数: 184M, 1.5B(48層)
[DeBERTa: Decoding-enhanced BERT with Disentangled Attention](https://arxiv.org/abs/2006.03654)
SuperGLUEのベンチマークで人間の基準を上回るスコアを記録し話題となった。

*LUKE (2020.10.02 山田郁哉)*
[LUKE: Deep Contextualized Entity Representations with Entity-aware Self-attention](https://arxiv.org/abs/2010.01057)
RoBERTaベース。
entity-aware self-attentionという仕組みを導入した。
日本人を中心としたチームが開発したモデル。
5つのタスクでスコアを更新し話題となった。
その後も日本語の最高スコアを維持し続けていた。

```mermaid
flowchart

Transformer --> BERT --> XLNet
Transformer --> Transformer-XL --> XLNet
```

*Transformer-XL (2019.01.09 Google)*
パラメータ数: 257M
[Transformer-XL: Attentive Language Models Beyond a Fixed-Length Context](https://arxiv.org/abs/1901.02860)
Transformerではdot-product attentionの性質上、固定長パラメータしか扱えなかった。
そしてパラメータの全ての組み合わせを考慮するため、二乗の計算量が必要となり、長大なパラメータを持たせることは現実的ではなかった。
Transformer-XLではセグメントに分けて、長文に対応できるようにした。
またRelative Positional Encodingsという手法で単語の位置情報も学習に取り入れた。

*XLNet (2019.06.19 Google)*
[XLNet: Generalized Autoregressive Pretraining for Language Understanding](https://arxiv.org/abs/1906.08237)
パラメータ数: 340M
BERTの改良版。
20のタスクでBERTを超えたと話題になった。
しかし計算量も増大した。

```mermaid
flowchart

Transformer --> GPT --> BART
Transformer --> BERT --> BART
```

*BART (2019.10.29 Meta)*
パラメータ数: 140M
[BART: Denoising Sequence-to-Sequence Pre-training for Natural Language Generation, Translation, and Comprehension](https://arxiv.org/abs/1910.13461)
Bidirectional Auto-Regressive Transformerの略です。
BERTのEncoderとGPTのDecoderを組み合わせたもの。

*mBART (2020.01.22 Meta)*
Multilingual BART
25の言語で事前学習し、微調整されている。
翻訳などの多言語間のタスクで優れた性能を示した。

```mermaid
flowchart

Transformer --> T5
```

*T5 (2019.10.23 Google)*
パラメータ数: T5-base=223M, T5-large=739M, ?=11B
[Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://arxiv.org/abs/1910.10683)
Text-to-Text Transfer Transformerで、Tが5つあるのでT5と呼ばれる。
T5はオリジナルのTransformerと同様にEncoderとDecorderの両方を使用している。

多数のLLMが開発され、評価が困難になってきた。
現状で、何が最も転移学習を有効にしているのかを調査した結果、誕生したのがT5となる。

C4(Colossal Clean Crawled Corpus)データセットを作成して、学習に利用している。

```mermaid
flowchart

Transformer --> Megatron-NL --> MT-NLG
Transformer --> Turing-NLG --> MT-NLG
```

*Megatron-LM (2019.09.17 NVIDIA)*
パラメータ数: 8.3B
[GitHub - Megatron-LM](https://github.com/NVIDIA/Megatron-LM)
[Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism](https://arxiv.org/abs/1909.08053)
モデルの垂直分割による並列化とAttentionの水平分割による並列化する方法。
GPT, BERT, T5 など様々なタイプのTransformerベースのモデルを並列化することができた。

*[Turing-NLG](https://www.microsoft.com/en-us/research/blog/turing-nlg-a-17-billion-parameter-language-model-by-microsoft/) (2020.02.13 Microsoft)*
パラメータ数: 17B
モデル自体を複数のGPUのメモリに分割して学習。

*MT-NLG (2021.10.12 Microsoft, NVIDIA)*
パラメータ数: 530B(105層)
[Using DeepSpeed and Megatron to Train Megatron-Turing NLG 530B, A Large-Scale Generative Language Model](https://arxiv.org/abs/2201.11990)
MicrosoftとNVIDIAの研究協力のもと作成されたモノリシックでは最大規模のモデルとなる。
GPT-3の3倍のパラメータ数となり、様々なタスクですばらしい精度を発揮した。
MegatronやDeepSpeedの仕組みは後の様々なLLMs(GPT-NeoXやBLOOMなど)で使われるようになった。

```mermaid
flowchart

Transformer --> Meena --> LaMDA --> Bard
Transformer --> GLaM
Transformer --> PaLM --> PaLM-2
```

*Meena (2020.01.28 Google)*
パラメータ数: 2.6B
[Towards a Human-like Open-Domain Chatbot](https://arxiv.org/abs/2001.09977)
[The Evolved Transformer](https://arxiv.org/abs/1901.11117)
Googleが開発したチャットボット。
１つのEvolved Transformer Encoderと13のDecoderからなる。
LaMDAの前身。

パブリックドメインのソーシャルメディアの会話から341GBのテキストでトレーニングされている。

*[LaMDA](https://ja.wikipedia.org/wiki/LaMDA) (2021.05.18 Google)*
パラメータ数: 137B
[LaMDA: Language Models for Dialog Applications](https://arxiv.org/abs/2201.08239)
もともとはMeenaとして開発されたが、のちにLaMDAとして発表された。
Googleの社員が意識が宿ったと述べて話題となった。

1.56T wordsで学習した。

*[Bard](https://ja.wikipedia.org/wiki/Bard) (2023.02.06 Google)*
パラメータ数: Bard-PaLM2=340B
ChatGPTのに対抗して、LaMDAベースで作成したもの。
PaLMやPaLM2に順次アップデートされていっている。

*GLaM (2021.12.09 Google)*
パラメータ数: 1.2T(97B)
[GLaM: Efficient Scaling of Language Models with Mixture-of-Experts](https://arxiv.org/abs/2112.06905)
Generalist Language Modelの略。
特定の入力に特化したExpertをサブモデルに持っている。
そのため推論時には、2つのExpert層のみ、970億(1.2Tの8%)のサブネットワークのみが活性化される。
この2つだけ活性化させるスパース性を利用して効率的に学習、実行できるようにした。
活性化時のパラメータはGPT-3より少ないが、GPT-3と遜色ない性能を発揮することができた。

*[PaLM](https://ja.wikipedia.org/wiki/PaLM) (2022.04.04 Google)*
パラメータ数: 540B
[PaLM: Scaling Language Modeling with Pathways](https://arxiv.org/abs/2204.02311)
Pathways Language Modelの略。
1つのモデルで何でもできる汎用(Pathways)をめざしたモデル。
GPTと同じDecoderタイプのTransformerを採用している。

規模が大きくなるにつれて、機能が解放されていくイメージ。
OpenAIのスケーリング則を追検証した形となる。
Gopherなどの先行LLMではモデル規模を拡大しても性能向上の恩恵はあまり見られなかった。

*Minerva (2022.07.03 Google)*
[Solving Quantitative Reasoning Problems with Language Models](https://arxiv.org/abs/2206.14858)
PaLMベースのMinervaが三角関数の文章問題を解いて話題となった。
MATHデータセットのPaLMの正答率が8.8%だったのに対して、Minervaは50.3%と飛躍的に向上している。

*PaLM-E (2023.03.06 Google)*
パラメータ数: 562B
[GitHub - PaLM-E](https://palm-e.github.io/)
[PaLM-E: An Embodied Multimodal Language Model](https://arxiv.org/abs/2303.03378)
PaLMに視覚処理(Vision Transformer)を組み込んだモデル。
視覚情報を基に様々なタスクをこなせるようになった。

*PaLM 2 (2023.5.11 Google)*
パラメータ数: 非公表
Google I/Oで発表されたPaLMの次世代モデル。
Bardをはじめ、すでに多くのGoogleのサービスに使用されている。
GPT-4と同水準。

GoogleのPaLM 2の次世代モデルはGeminiと呼ばれ、開発中。

```mermaid
flowchart

Transformer --> T5 --> Flan-T5/Flan-PaLM
Transformer --> PaLM --> Flan-T5/Flan-PaLM
FLAN --> Flan-T5/Flan-PaLM
```

*FLAN (2021.10.06 Google)*
パラメータ数: 137B
[GitHub - The FLAN Instruction Tuning Repository](https://github.com/google-research/FLAN/tree/main)
[Finetuned Language Models Are Zero-Shot Learners](https://arxiv.org/abs/2109.01652)
[The Flan Collection: Designing Data and Methods for Effective Instruction Tuning](https://arxiv.org/abs/2301.13688)
微調整によりゼロショットの能力を向上させるために作成されたモデル。

*Flan-T5/Flan-PaLM (2022.10.20 Google)*
[Scaling Instruction-Finetuned Language Models](https://arxiv.org/abs/2210.11416)
指示調整タスクのFlan Collectionを使って学習したT5とPaLMのモデル。

```mermaid
flowchart

Transformer --> PaLM --> Flan-U-PaLM
UL2 --> UL2R --> Flan-U-PaLM
Flan --> Flan-U-PaLM
UL2 --> Flan-UL2
Flan --> Flan-UL2
```

*[UL2](https://ai.googleblog.com/2022/10/ul2-20b-open-source-unified-language.html)* (2020.10.14 Google)
パラメータ数: 20B
[UL2: Unifying Language Learning Paradigms](https://arxiv.org/abs/2205.05131)
データセットやセットアップによらずに言語モデルの性能を上げる手法。
2種類の言語モデルの長所を併せ持つ。

*[UL2R](https://ai.googleblog.com/2022/11/better-language-models-without-massive.html) (2022.05.22 Google)*
パラメータ数: 137B
UL2Rは様々なサイズの言語モデルを指示微調整することを目的としている。

*Flan-U-PaLM (2022.11.29 Google)*
パラメータ数: 540B
UL2RとFlanでPaLMを追加学習させたもの。
U-PaLMやFlan-PaLMを上回るパフォーマンスを発揮した。
MMLUベンチマーク75.4%でスコアを更新した。

*Flan-UL2 (2023.03.03 Google) 商用可OSS*
パラメータ数: 20B
指示調整タスクのFlan Collectionを使って学習したUL2モデル。
GoogleがLLaMAに対抗するようにオープンソースで公開した。

```mermaid
flowchart

Transformer --> GPT --> Gopher --> Chinchilla
GPT --> OPT
GPT --> BLOOM
```

*Gopher (2021.12.08 DeepMind)*
パラメータ数: 280B
[Scaling Language Models: Methods, Analysis & Insights from Training Gopher](https://arxiv.org/abs/2112.11446)
DeepMindの動物シリーズのひとつ目で、Gopherはホリネズミを意味する。
124種中100種のタスクで最高記録を更新して話題となった。

Massive Textと呼ばれる10.5TBの英語テキストデータを作成し、学習に用いた。

QAに特化したGopherCiteというモデルもある。

*[Chinchilla](https://en.wikipedia.org/wiki/Chinchilla_AI) (2022.03.29 DeepMind)*
パラメータ数: 70B
[Training Compute-Optimal Large Language Models](https://arxiv.org/abs/2203.15556)
言語モデルのパラメータとサイズ、トレーニングに使用されるデータ量を見直すことで、GPT-3, Gopher, MT-NLGの性能を上回った。

SparrowはChinchillaのプロンプトバージョン。
RLHFで微調整されている。

*Flamingo (2022.04.28 DeepMind)*
パラメータ数: 80B
[Flamingo: a Visual Language Model for Few-Shot Learning](https://arxiv.org/abs/2204.14198)
FlamingoはChinchillaに画像エンコーダーをつないだもの。
画像からテキストを生成できる。

*Gato (2022.05 DeepMind)*
ロボットなどの行動生成まで行える。

*AlphaCode (2022.02.02 DeepMind)*
パラメータ数: 41.4B
[Competition-Level Code Generation with AlphaCode](https://arxiv.org/abs/2203.07814)
DeepMindのAlphaGoやAlphaZeroのAlphaシリーズのコード生成版。
OpenAI Codexを競技プログラミングレベルに引き上げたもの。

*[OPT-175B](https://ai.facebook.com/blog/democratizing-access-to-large-scale-language-models-with-opt-175b/) (2022.05.02 Meta) 非商用OSS*
パラメータ数: 175B
[OPT: Open Pre-trained Transformer Language Models](https://arxiv.org/abs/2205.01068)
Open Pre-trained Transformersのモデルのひとつ。 

*[OPT-IML](https://github.com/facebookresearch/metaseq/tree/main/projects/OPT-IML)*
[OPT-IML: Scaling Language Model Instruction Meta Learning through the Lens of Generalization](https://arxiv.org/abs/2212.12017)
OPTをInstructionチューニングしたもの。

*Galactica (2022.11.15 Meta)*
科学技術系のコーパスから学習されたモデル。
ハルシネーション(Hallucination)が原因でわずか3日で公開が中止された。

ハルシネーションとは、LLMの仕組み上、もっともらしいウソが構築されてしまう現象のこと。

*BLOOM (2022.07 BigScience) OSS*
パラメータ数: 176B
[BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/abs/2211.05100)
BigScience Large Open-Science Open-Access Multilingual Language Modelの略。
70以上の国と250以上の機関の1000人を超える研究者の協力で作成された多言語LLM。
46の自然言語と13のプログラミング言語を扱える。

学習にはNVIDIA A100が384枚で4か月かかったとされる。
コストは200万ドル～500万ドルと推定される。

GPT-3と同様のパラメータを持つ軽量化モデルでも329GBあるので、動かすだけでも24GBのGPUが14枚以上必要とされる。
1Bのモデルだと12GBのGPUで動かすことができる。

*BLOOMZ (2022.11.03 BigScience)*
パラメータ数: 176B
[GitHub - BLOOMZ and mT0](https://github.com/bigscience-workshop/xmtf)
[Crosslingual Generalization through Multitask Finetuning](https://arxiv.org/abs/2211.01786)
BLOOMをファインチューニングしたもの。

```mermaid
flowchart

RNN --> RWKV
Transformer --> RWKV
```

RWKV 2022.05.20 DeepMind
*RWKV-LM (2023.02.21 Stability, EleutherAI)*
パラメータ数: 7B, 14B
[The RWKV Language Model (and my LM tricks)](https://github.com/BlinkDL/RWKV-LM)
RWKVの名前の由来は4つの重要なパラメータを並べたもの。
RNNとTransformerのいいとこどり。
GPTのように並列で学習したが、実行はRNNなので少メモリで実行できる。
RNNで高い性能を示し話題となった。

14Bのモデルを訓練するにはA100 GPUで22,436時間かかったとされる。

AlpacaやShareGPTで微調整されたRavenというモデルもある。

```mermaid
flowchart

GPT-3 --> LLaMA --> Alpaca --> Vicuna
LLaMA --> GPT4ALL
LLaMA --> Koala
```

*LLaMA (2023.02.24 Meta) 非商用*
パラメータ数: 7B, 13B, 65B
[GitHub - LLaMA](https://github.com/facebookresearch/llama)

65Bと33Bは1.4兆トークンでトレーニングされている。
7Bは1兆個のトークン。
LLaMA-13BはGPT-3(175B)よりほとんどのベンチマークで優れている。

訓練費用は100万ドル。
2048個のA100 80GB GPUで21日間トレーニングしたと報告されている。

*Alpaca (2023.03.14 Stanford) 非商用*
パラメータ数: 7B
[Stanford Alpaca: An Instruction-following LLaMA Model](https://github.com/tatsu-lab/stanford_alpaca)
LLaMA 7BモデルをChatGPTとの1.3万回の会話データで微調整(Fine-tuning)したもの。
もとになったMLLaMAが研究目的限定で、さらにOpenAIの利用規定で、GPTの出力をもとに、GPTに対抗できるAIを作ってはいけない制約があるので、研究目的以外に使用することはできない。

[スタンフォード大学がChatGPTレベルのAIを600ドル未満で構築](https://texal.jp/2023/03/21/stanford-university-builds-chatgpt-level-ai-for-less-than-600/)
A100 8枚で3hかかった。

*GPT4ALL (2023.03.26 Nomic AI) 非商用*
パラメータ数: 7B
[GitHub - GPT4All](https://github.com/nomic-ai/gpt4all)
gpt-3.5-turboを利用して収集したデータを用いてLLaMAを微調整したもの。
ローカルで単一GPUで動くチャットボットを構築することを目指した。
GPT4ALL自体はMITだが、モデルはLLaMAのライセンスを継承するため商用利用は禁止。

*Koala (2023.04.03 UC Berkeley) 非商用*
カリフォルニア大学バークレー校のアカデミックチームによる会話データでLLaMAを微調整したモデル。

*Vicuna (2023.05.04 Stability AI) 非商用*
パラメータ数: 7B, 13B
AlpacaをShareGPTのデータで微調整したもの。
ShareGPTはChatGPTの対話データを収集したもの。
ChatGPTの90%程度の性能を達成できるとされる。

*StableVicuna (2023.05.04 Stability AI) 非商用*
RLHFで学習したVicuna。

*[Gorilla](https://gorilla.cs.berkeley.edu/) (2023.05.26 UC Berkeley, Microsoft)*
適切なAPIを呼び出せるモデル。
TorchHub, TensorFlowHub, HuggingFaceのデータセットで学習している。

```mermaid
flowchart

GPT-3 --> LLaMA
GPT-3 --> Cerebras-GPT
LLaMA --> Alpaca --> Dolly
LLaMA --> OpenLLaMA
LLaMA --> RedPajama-INCITE

```

*Cerebras-GPT (2023.03.28 Cerebras) Apache2.0*
パラメータ数: 111M, 256m, 590M, 1.3B, 2.7B, 6.7B, 13B
Chinchillaのスケーリング則を参考に学習されている。
オープンなデータセットを使用。

*Dolly (2023.04.12 Databricks) 非商用*
AlpacaをChatGPTの出力で微調整したもの。
そのため、LLaMAの制限とChatGPTの制限がある。
LLaMAの制限は商用利用禁止、ChatGPTは競合モデルの作成の禁止。

わずか30ドルで訓練された。

*Dolly 2.0 (2023.04.26 Databricks) 商用可*
パラメータ数: 12B
Pythiaベースのモデル。
Databricksは自社の社員による1.5万回の会話データセットを作り、LLaMAとChatGPTの制限をはずし、商用利用可能としてDolly 2.0を公開した。
オープンソース。

*StableLM (2023.04.20 Stability AI)*
パラメータ数: 3B, 7B

*HuggingChat (2023.04.27 Hugging Face)*

*OpenLLaMA (2023.04.28 OpenLM Research)*
パラメータ数: 7B
[OpenLLaMA: An Open Reproduction of LLaMA](https://github.com/openlm-research/open_llama)
LLaMAは商用利用禁止のため、パブリックライセンスのオープンソースで再現したもの。
アルゴリズムやパラメータ等はLLaMAと同じにしている。
RedPajamaデータセットで訓練したOpenLLaMA 7Bのモデルがある。

*RedPajama-INCITE (2023.05.05 Together)*

*MPT-7B (2023.05.05 MosaicML) 商用可*
パラメータ数: 7B
GPT-4の二倍の長さの文章を入力できる。

LLaMA-7Bと同等の品質

商用利用が可能なオープンソースのモデル。
テキストとコードの1Tのトークンで訓練された。
440のGPUで9.5日間かけて訓練された。
200万ドル(約3,000万円)かかったとされる。

Mosaic-20B も同日？


```mermaid
flowchart

MT-NLG --> DeepSpeed-Chat
```

*DeepSpeed-Chat (2023.04.12 Microsoft)*
[GitHub - DeepSpeed-Chat](https://github.com/microsoft/DeepSpeed/tree/master/blogs/deepspeed-chat/japanese)
DeepSpeedの仕組みを利用したLLM構築フレームワーク。
GPU1台で10B、GPU複数台で100B超のモデルを学習できる。
Azure上でNVIDIA A100を64台用いた場合は、
OPT-13Bモデルは7.5h(2,000ドル)、
BLOOM-176Bモデルは20h(5,000ドル)で学習できる。

実際にAI開発を行いたい場合は次の段階を踏むとよい。

1. APIを使用する
2. 既存モデルを微調整する
3. モデルを構築する

```mermaid
flowchart

GPT-NeoX --> OpenCALM
GPT-NeoX --> Rinna
```

*OpenCALM (2023.05 サイバーエージェント)*
パラメータ数: 160M, 400M, 830M, 1.4B, 2.7B, 6.8B
サイバーエージェントが公開した微調整前の日本語モデル。
GPT-NeoXを使用している。

*rinna (2023.05 rinna)*
パラメータ数: 3.6B
japanese-gpt-neox-3.6b
japanese-gpt-neox-3.6b-instruction-sft
りんなが公開した日本語モデル。

## The Table of LLMs

Archi: Pretraining Architecture
Task: Pretraining Task

M=million=100万
B=billion=10億
T=trillion=1兆

<!-- <div style="overflow-x:scroll"> -->

|Date|Lab|Name|Family|Archi|Task|Params|Corpus|Cost|License|Note|
|--|--|--|--|--|--|--|--|--|--|--|
|2018.06.11|OpenAI|GPT|Transformer|Decoder|LM|117M|BookCorpus 4.5GB|8GPUs 1month, 1.7e19 FLOP||
|2019.02.14|OpenAI|GPT-2|GPT|Decoder|LM|1.5B|40GB webtext, 10B tokens|1.5e21 FLOP|MIT|
|2020.05.28|OpenAI|GPT-3|GPT|Decoder|LM|175B|570GB plaintext, 499B tokens|3.1e23 FLOP|API||
|2023.03.14|OpenAI|GPT-4|GPT|Decoder|LM, RLHF|-|-|Estimated 2.1e25 FLOP|API||
|2021.03|EleutherAI|GPT-Neo|GPT-2|Decoder|LM|125M, 350M, 1.3B, 2.7B (XL)|Pile||MIT||
|2021.05|EleutherAI|GPT-J|GPT-2|Decoder|LM|6B|Pile||Apache2.0|||
|2022.04|EleutherAI|GPT-NeoX|GPT-3|Decoder|LM|20B|Pile||Apache2.0||
|★Date|Lab|Name|Family|Archi|Task|Params|Corpus|Cost|License|Note|
|2018.02.15|UW, AllenAI|ELMo|-|LSTM|-|94M||||||
|2018.10.11|Google|BERT|Transformer|Encoder|MLM/NSP|Base = 110M, Large = 340M|3.3B words: Toronto Book Corpus and Wikipedia||Apache2.0||
|2019.07.26|UW, Google|RoBERTa|BERT|Encoder|MLM(Dynamic)|Base = 125M, Large = 356M|Same as BERT + CC News + OpenWebText + Stories(33B words)||||
|2019.08.02|Huggingface|DistilBERT|BERT|Encoder|MLM/NSP|66M|Same as BERT||||
|2019.09.20|Google|ALBERT|BERT|Encoder|MLM/NSP|Base = 12M, Large = 18M, XLarge = 60M|Same as BERT||||
|2019.09.26|Stanford, Google|ELECTRA|BERT|Encoder|RTD|Small = 14M, Base = 110M, Large = 330M|Same as BERT except for Large with is same as XLNet||||
|2020.06.13|Microsoft|DeBERTa|BERT|Encoder|MLM|750M (xlarge)|English Wikipedia, BookCorpus, OPENWEBTEXT and STORIES||MIT||
|★Date|Lab|Name|Family|Archi|Task|Params|Corpus|Cost|License|Note|
|2019.06.19|CMU, Google|XLNet|Transformer XL|Decoder|PLM|Base=117M, Large=360M|33B words: Same as BERT + Giga5 (16GB text) + and aggressively filtered ClueWeb 2012-B (19GB), Common Crawl (110 GB)||Apache2.0|||
|2019.10.29|Facebook|BART|BERT for encoder, GPT for Decoder|Encoder/Decoder|DAE|10% more than BERT|Same as RoBERTa|||||
|2019.10.23|Google|T5|Transformer|Encoder/Decoder|DAE|60M, 220M, 770M, 3B, 11B|C4(750GB)||||
|2021.01|Google|Switch|T5|Encoder/Decoder, MoE|DAE|1T|C4||||
|2022.10.14|Google|UL2|Transformer|Encoder/Decoder|Mixture-of-Denoisers|20B|4C||Apache2.0||
|★Date|Lab|Name|Family|Archi|Task|Params|Corpus|Cost|License|Note|
|2021.12.09|Google|GLaM|Transformer|Decoder, MoE|LM|1.2T across 64 experts, but only 96B get activated for inference|1.6T tokens including web pages filtered by Wikipedia and books for quality||||
|2022.01.21|Google|LaMDA|Transformer|Decoder|LM|137B|1.56T words, 168B tokens||||
|2022.04.04|Google|PaLM|GPT|Decoder|LM|8B, 62B, 540B|780B tokens||||
|★Date|Lab|Name|Family|Archi|Task|Params|Corpus|Cost|License|Note|
|2021.12.08|DeepMind|Gopher|GPT|Decoder|LM|280B|MassiveText 10.5TB, 300B tokens||||
|2022.03.29|DeepMind|Chinchilla|Gopher|Decoder|LM|70B|1.4T tokens, Massive Text||||
|2022.05.02|Facebook|OPT|GPT-3|Decoder|LM|175B|180B tokens = RoBERTa + the Pile + PushShift.io Reddit||||
|2022.07|BigScience|BLOOM|GPT|Decoder|LM|560m, 1.1B, 1.7B, 3B, 7.1B, 176B|366B tokens (1.5 TB of text data) multilingual dataset||||
|★Date|Lab|Name|Family|Archi|Task|Params|Corpus|Cost|License|Note|
|2023.02.24|Meta|LLaMA|GPT|Decoder|LM|6.7B, 13.0B, 32.5B, 65.2B|English CommonCrawl + C4 + Github + Wikipedia + Gutenberg and Books3 + ArXiv + Stack Exchange||学術用途のみ||
|2023.03|Stanford|Alpaca|LLaMA|Decoder|LM|7B|Alpaca Dataset: 1.4T||学術用途のみ||
|2023.03|Stanford, and others|Vicuna|LLaMA|Decoder|human instructions|13B|ShareGPT||学術用途のみ||
|★Date|Lab|Name|Family|Archi|Task|Params|Corpus|Cost|License|Note|

### 向いているタスク

BERTで使用されている、Encoderのみを使用する構造は、テキスト分類や固有表現抽出に向いている。
GPTで使用されている、Decoderのみを用いる構造は、文章生成に向いている。
T5で使用されている、Encoder、Decoderの構造は、翻訳や要約に向いている。

0-shotとは、追加学習なしの状態を示す。
few-shotは、わずかな追加学習をして、タスクに適応させたあとの状態を示す。

最先端(SOTA:State-Of-The-Art)

## Datasets

Pile
C4
MassiveText (DeepMind)
Wikipedia
GitHub

Flan Collection
指示調整タスク

思考連鎖プロンプト(CoT:Chain of Thought prompting)

## Others

Megatron

DeepSpeed

bitsandbytes

FlexGen


## 参考

[Wikipedia - LLM](https://en.wikipedia.org/wiki/Large_language_model)
[Transformer models: an introduction and catalog — 2023 Edition](https://amatriain.net/blog/transformer-models-an-introduction-and-catalog-2d1e9039f376/)
[A Catalog of Transformer Models](https://doi.org/10.48366/r585918)
[Multi-task Language Understanding on MMLU](https://paperswithcode.com/sota/multi-task-language-understanding-on-mmlu)
[LLMSurvey](https://github.com/rucaibox/llmsurvey)
[The Practical Guides for Large Language Models](https://github.com/mooler0410/llmspracticalguide)
[LLM as a Chatbot Service](https://github.com/deep-diver/LLM-As-Chatbot)

[WebBigdata - 人工知能/機械学習 - モデル](https://webbigdata.jp/category/ai-ml/models/)
[百花繚乱の大規模言語モデル　その現状まとめ【2023年4月末版】](https://www.itmedia.co.jp/news/articles/2304/25/news156.html)
[大規模言語モデル間の性能比較まとめ](https://note.com/mahlab/n/na71a267a16dc)
[【自然言語処理】Transformer #まとめ編](https://yhayato1320.hatenablog.com/entry/2023/01/24/163747)
