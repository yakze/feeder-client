# Feeder Chat Electron Client 🚀

> HOLY🪽 client

## 🧠 What's Feeder Chat?

Feeder Chatは、軽量でリアクティブなチャットシステム。  
このElectronクライアントは、その"プレーンで静かなUI"に美学を込めて設計された、デスクトップ専用アプリケーションです。

- ⛓️ **リアルタイム通信**：WebSocketベースの高速通信
- 🌓 **ダーク&ライトテーマCSS**：システム連動、自動切り替え
- 🔒 **安全設計**：コンテンツセキュリティポリシーとIPC分離
- 🧩 **Plugin-friendly**：機能拡張のためのAPI設計済み

---

## ✨ Design Philosophy

- **安全性**： Electron製のプライバシー重視なWebsocketフレーム設計
- **機能性**：worst連携機能及び17個の基本装備機能
- **拡張性**：外部スクリプトの簡単な注入

---

## 🛠️ Built With

　| Tech          | Role                          |
　|---------------|-------------------------------|
　| Electron      | クロスプラットフォーム基盤     |
　| React + Vite  | フロントエンド高速構築         |
　| Tailwind CSS  | 美しく、柔軟なUI構築           |
　| TypeScript    | 安定性と可読性の両立           |
　| WebSocket     | リアルタイム通信               |

---

## ⚡ Features

- ✅ 軽量・高速起動（1秒以内に初期描画）
- ✅ 設定不要、起動即ログイン（トークン自動管理）
- ✅ ドラッグ＆ドロップでファイル送信
- ✅ 通知連携（バッジ/デスクトップ通知）
- ✅ ショートカット対応（Cmd/Ctrl + Kでチャンネル切替）
- ✅ Markdownレンダリング + カスタム絵文字
- ✅ ADblock（広告非表示）
- ✅ 完全無視機能　（返信セクション内無視貫通防止）
- ✅ 5個のフリーアカウント（＋版は15個）
- ✅ ALTmanager（サブ垢管理）
- ✅ カスタムCSSローダー
- More…

---

## 🚧 Project Structure

feeder-client-electron/
<b>├── public/ # アイコン・マニフェスト
<b>├── src/
<b>│ ├── main/ # Electron メインプロセス
<b>│ ├── renderer/ # フロントエンド（React）
<b>│ └── preload.ts # 安全なブリッジスクリプト
<b>├── dist/ # ビルド成果物
<b>├── package.json
<b>├── vite.config.ts
<b>└── electron-builder.yml

## 🚀 Getting Started

```bash
git clone https://github.com/yourname/feeder-client-electron
cd feeder-client-electron
npm install
npm run dev
```
💡 npm run buildでバイナリ出力（macOS/Windows/Linux対応）

```ts
// tailwind.config.ts
theme: {
  extend: {
    colors: {
      primary: '#00BCD4',
      surface: 'var(--color-surface)',
    }
  }
}
```
＞自動でOSのテーマを検出し、カスタム変数へバインド。
＞ユーザーによる強制テーマ設定も可能（settings.jsonに保存）。

## 🔐 Security
contextIsolation: true + preload.jsによる厳格なIPC
Rendererプロセスは直接Node APIに触れない構成
全通信はSSL/TLSで暗号化（WebSocket + HTTPS）
## 🤝 Contribution
1. Forkする
2. 新しいブランチを切る
3. 修正してPRを出す（詳細な説明つけてくれると助かります）

## 📦 Packaging
```bash
npm run build
npm run make
```
>Electron Builder を使用して各OSに対応したインストーラを生成します。

## 📄 License
MIT License

## 🧭 Credits
Crafted with care by @yakze & ロリ幼女（組織）
Feederプロトコルは Feeder.info によって設計されています




