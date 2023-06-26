# links

[OpenAI](https://openai.com/)
ChatGPT API, Wisper API

## Speech to text


## Text to speech

有償でよければVOICEPEAKが無調整で一番自然な感じがする。

### 無料

[VOICEVOX](https://voicevox.hiroshiba.jp/)
クレジット表示必要。
TTSController(内部的にはREST API呼び出し)に対応。
公式で REST API に対応。

[COEIROINK](https://coeiroink.com/)
GUIにVOICEBOXをカスタムしたものを使用している。
エンジンは別物。
TTSController(VOICEVOXと同じ)に対応。

[音読さん](https://ondoku3.com/ja/)
クレジット表示必要。
ChatGPTのレスポンスを読み上げてくれるChrome拡張がある。

[SpeechSynthesis](https://developer.mozilla.org/ja/docs/Web/API/SpeechSynthesis)
ブラウザの音声合成

[棒読みちゃん](https://chi.usamimi.info/Program/Application/BouyomiChan/)

[SofTalk](https://w.atwiki.jp/softalk/)

[テキストーク](https://gui.jp.net/textalk/)

### 有償パッケージ

[VOICEPEAK](https://www.ah-soft.com/voice/narrator/)
TTSController(内部的にはコマンドラインからのwav作成)に対応。
未調整でもそれなりの品質になる。
商用ナレーターセットは、商用利用できるが、それ以外は別途商用ライセンスが必要。

邪神ちゃん無料お試し版があるが制限がある。
標準音声のみ、100文字、5ブロックまでとなっている。

古い製品にVOICEROID、VOICEROID2があるが、そちらは違和感が残る音声となっている。

[CeVIO AI](https://cevio.jp/)
チェビオと読む。
TTSController(.NETアセンブリ呼び出し)に対応。
公式で .NET Framework 4.8 に対応。
DLL名は CeVIO.Talk.RemoteService2.dll となる。

2013年からCeVIO CS(Creative Studio)として発売されている。
姉妹ソフトとしてOpen JTalkとSinsyがある。
CeVIO AIの姉妹ブラントとしてVoiSona(旧CeVIO Pro(仮称))がある。

[A.I.VOICE](https://aivoice.jp/)
AITalk5の技術を使用している。
かんたん！AITalk5というソフトもある。
TTSController(.NETアセンブリ呼び出し)に対応。
公式で .NET Framework 4.7.2 に対応。
DLL名は AI.Talk.Editor.Api.dll となる。

[AquesTalk](https://www.a-quest.com/products/aquestalk.html)
組み込みに使えるほど小型。

### サブスク

[CoeFont](https://coefont.cloud/)
リアルタイムには遅いか？

[Azure Speech Service](https://learn.microsoft.com/ja-jp/azure/cognitive-services/speech-service/language-support?tabs=stt)

[Google Text-to-Speech](https://cloud.google.com/text-to-speech?hl=ja)

[Amazon Polly](https://aws.amazon.com/jp/polly/)

## Others

Semantic Kernel

LangChain

AutoGPT

AgentGPT

HuggingGPT

BabyAGI

CAMEL

JARVIS

## Libraries

[Azure OpenAI Service の C# SDK (ChatGPT でも使えます)](https://zenn.dev/microsoft/articles/azure-openai-service-csharpsdk)

[marcominerva/ChatGptNet](https://github.com/marcominerva/chatgptnet)

[wieslawsoltes/ChatGPT](https://github.com/wieslawsoltes/chatgpt)

[ksasao/TTSController](https://github.com/ksasao/TTSController)
VOICEVOX, COEIROINK, VOICEPEAK, CeVIO AI, A.I.VOICEなどを統一的に扱うライブラリ。

## Refers

[Gortana GPT - Voice Chat Interface](https://github.com/dasdata/gortanagtp)
Azure Cognitive Services
OpenAI ChatGPT

[Unity VOICEVOX Bridge](https://github.com/mikito/unity-voicevox-bridge)
VOICEVOX

[ChatdollKit](https://github.com/uezo/ChatdollKit/blob/master/README.ja.md)
Unity

[Whisper API, ChatGPT API, VOICEVOXを使ってAIと会話する](https://zenn.dev/umyomyomyon/articles/5f07abe67a289b)

[ChatGPTキャラクターマスコットアプリの紹介【準備＆インストール編】](https://qiita.com/Haruyama_Dev/items/d03cd30b80d96697db2c)

[VOICEVOXをC#でREST-API経由で喋らせる（その１　発話）](https://qiita.com/oyahun/items/e01e56878dc011cdc094)

[A.I.VOICE Editor API](https://aivoice.jp/manual/editor/api.html)

[ChatGPTでキャラを動かそう！キャラ再現率が高いプロンプトと回答をしっかり縛れるAPIフロー](https://zenn.dev/niwatoro/articles/180f6185c382bb)

[チャット欄に答えて雑談配信する「AI VTuber」の作り方](https://zenn.dev/makunugi/articles/a4ed9e142526f2)


