```mermaid
flowchart TD
  A[Onload] -- 無反応 --> B(...);
  A -- こんにちは --> C[相手の名前を呼んで今日のおすすめを案内する];
  A -- はじめまして --> D[自分の名前を名乗って会話パターンを案内する];
  B -- トークデッキ --> E[トークデッキ];
  E -- 無反応 --> B;
  D -- おすすめは何 --> C;
  C -- トークデッキ --> E;
  A -- できることは何 --> D;
  C -- AIの仕組み -->F[AIの仕組み概要];
  F -- Watson Assistantは何 -->G[Watson Assistantの説明];
  G -- rinna GPT-2は何 --> H[rinna GPT-2の説明];
  H -- WebSocketは何 --> I[WebSocketの説明];
  I -- Three-VRMは何 --> J[Three-VRMの説明];
  J -- VRoidは何 --> K[VRoidの説明];
  K -- Watson Assistantは何 -->G;
