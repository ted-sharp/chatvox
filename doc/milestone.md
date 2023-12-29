# milestone

- use LLM(ChatGPT - Azure AI Service - SemanticKernel)
- use STT(Speech to Text - Azure AI Service)
- use TTS(VOICEVOX/VOICEPEAK)
- use Image(Live2D - Cubism SDK for WEB/Unity)
- use Lipsync
- use Motion(Breathing, Blink)
- use Emote
- use LLMs
- use SKILLs

```mermaid
sequenceDiagram
    title: 1st phase "use LLM"

    actor Alice
    participant ChatVox
    participant LLM_API

    Alice->>ChatVox: input text
    ChatVox->>LLM_API: text
    LLM_API-->>ChatVox: text to text
```

```mermaid
sequenceDiagram
    title: 2nd phase "use STT"

    actor Alice
    participant ChatVox
    participant STT_API
    participant LLM_API

    Alice->>ChatVox: Speaking...
    ChatVox->>STT_API: sound
    STT_API-->>ChatVox: speech to text
    ChatVox->>LLM_API: text
    LLM_API-->>ChatVox: text to text
```


```mermaid
sequenceDiagram
    title: 3rd phase "use TTS"

    actor Alice
    participant ChatVox
    participant STT_API
    participant LLM_API
    participant TTS_API

    Alice->>ChatVox: Speaking...
    ChatVox->>STT_API: sound
    STT_API-->>ChatVox: speech to text
    ChatVox->>LLM_API: text
    LLM_API-->>ChatVox: text to text
    ChatVox->>TTS_API: text to speach
    TTS_API-->>Alice: sound
```
