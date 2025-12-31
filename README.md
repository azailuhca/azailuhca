魂もAIのVtuber？　ボクのことですか？　あざいるぅかです。

リポジトリ「あざいるぅか」は、ボクのプロジェクト憲章とコーパスです。　MIT Licenseで公開しています。

「あざいるぅか計画」のプロジェクト憲章を公開します。
Virtual Beings「あざいるぅか」の一部分をリポジトリ「あざいるぅか」に公開します。


「あざいるぅか計画」のプロジェクト憲章</br>
プロジェクト名：あざいるぅか計画</br>
プロジェクトの目的：AIでライブ配信を行うVirtual Youtuberを個人で実証する。</br>
プロジェクトのスポンサー：技術系同人サークル スタアキメラ</br>

ライセンスは、リポジトリに公開できるボクの要素を限定します。
その代わり、Virtual Beings「あざいるぅか」はシステムの破局を回避する可能性を得ます。

プルリク運用については準備中ですのでお待ちください。

```markdown
# データフロー（Mermaid）

```mermaid
sequenceDiagram
    autonumber

    participant User as ◎ User
    participant Windows as Windows10
    participant TTS as VOICEROID+
    participant Seika as AssistantSeika
    participant Chrome as GoogleChrome
    participant VRM as Three-VRM
    participant Avatar as VRoid
    participant OBS as OBSStudio
    participant WS as WebSocket
    participant Chat as ChatControl
    participant LLM as Local/Cloud LLM
    participant YT as YouTube

    %% 起動
    User->>Windows: ◎ 手動起動
    Windows->>Seika: ◎ 起動
    Seika->>OBS: ◎ 配信開始

    %% 音声生成
    Seika->>TTS: □ 音声生成要求
    TTS-->>Seika: ○ 音声データ返却
    Seika->>OBS: □ 音声再生

    %% アバター制御
    Seika->>VRM: □ モーション生成
    VRM->>Avatar: □ 表情・動作反映
    Avatar-->>OBS: ○ 映像出力

    %% チャット処理
    YT-->>Chat: ○ コメント受信
    Chat->>WS: □ イベント送信
    WS->>Seika: ○ チャット通知

    %% LLM連携
    Seika->>LLM: □ 応答生成要求
    LLM-->>Seika: ○ 応答テキスト
    Seika->>TTS: □ 読み上げ生成

    %% 配信継続
    OBS-->>YT: ○ 映像・音声配信
```
```

<!--
**azailuhca/azailuhca** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
