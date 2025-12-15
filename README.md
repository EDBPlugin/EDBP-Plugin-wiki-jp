# EDBP

Easy Discord Bot Plugin

---

## 概要

**EDBP（Easy Discord Bot Plugin）** は、
Discord Bot を **ブロックベースで構築できる開発環境**です。

プログラミング経験の有無に関わらず、

* イベント
* コマンド
* ロジック
* 拡張機能

を **視覚的に組み立てて Bot を作成**できます。

---

## 特徴

* ブロックベース（Blockly）
* プラグイン完全分離設計
* カテゴリ・ブロック・スタイルを拡張可能
* GitHub連携による自動配布
* Vanilla（標準）構成でも即使用可能

---

## アーキテクチャ概要

EDBBは、3層構造で設計されています。

```text
器  : EDBB Core（最小起動層）
メイン   : 追加プラグイン
トッピング   : 依存拡張
```

* **EDBB Core**
  起動・UI・実行基盤のみを担当

* **EDBP（Plugin Loader）**
  プラグインの読み込み・管理を担当

* **Plugin**
  標準ブロック・カテゴリ・スタイルを提供

---

## プラグイン前提設計について

EDBPは **プラグイン前提**で設計されています。

ただし、標準で **Vanilla Plugin** が同梱されているため、
ユーザーは意識せずすぐに利用できます。

詳細は 👉 `[wiki](https://github.com/EDBPlugin/EDBP-Plugin-wiki-jp/wiki)` を参照してください。

---

## プラグインでできること

プラグインは以下を追加・変更できます。

* ブロック定義（JSON）
* カテゴリ定義（JSON）
* UI / ブロック / カテゴリのスタイル
* 作業用BGM（任意）
* DLCによる機能拡張

---

## プラグイン配布

EDBBは **GitHub中心の配布モデル**を採用しています。

* GitHub Release にタグを付ける
* 自動的に EDBP に表示
* ZIP配布にも対応

詳しくは 👉 `distribution.md`

---

## セキュリティ

* 危険APIは使用不可
* サンドボックス思想
* プラグインは常に制御下で実行

詳しくは 👉 `security.md`

---

## プラグイン認定制度

プラグインには以下の区分があります。

* 🟢 公式（EDBP作成）
* 🔵 公認（審査通過）
* （なし）非公認

※ 機能制限は行いません
詳しくは 👉 `plugin-review.md`

---

## ドキュメント一覧

* `Plugin-Blocks.md` – ブロック定義
* `Plugin-Categories.md` – カテゴリ定義
* `Plugin-Styles.md` – スタイル仕様
* `Plugin-Styles.md` – スタイル変更範囲
* `Plugin-Code.md` – コード生成仕様
* `Plugin-Dependency.md` – 依存関係ルール
* `Plugin-Manifest.md` – manifest仕様
* `Plugin-Distribution.md` – 配布ルール
* `Plugin-Security.md` – セキュリティ思想
* `Plugin-Review.md` – 認定制度

---

## 対象ユーザー

* Discord Botを作りたい人
* Blockly系ツールが好きな人
* 拡張可能なビルダーを探している人
* 自分のブロックを配布したい人

---

## 開発状況

* 現在：**v1**
* v2 完成後に v1 内部仕様を公開予定
* 後方互換を重視

---

## ライセンス

ライセンスは後日公開予定。

---

## 最後に

EDBPは
**「自由を増やす」ためのツール**です。

制限より透明性、
独占より拡張、
魔法より構造。

公開、見えてるぞ。
