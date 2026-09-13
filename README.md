# anchor-demo-vault

iOS アプリ **Anchor** のデモ用 vault（誰でも読める公開リポジトリ）。

アプリの接続画面の「アカウント無しで試す（デモ）」から、GitHub アカウントもトークンも無しで
このリポジトリを読み込めます（GitHub の REST API は公開リポジトリを未認証で読めるため）。

## 構造

カードの書式は Anchor Card Format v2。**ルールは <https://github.com/topo122/anchor-card-format/blob/main/SPEC.md> だけに書いてある**（ここには書かない）。

- `統計/基礎/` … 問題カード
- `統計/用語定義/` … `[[id]]` の参照先（＝定義の正本）。他のカードから参照され、表示時に展開される
- `統計/演習/` … 表と引用を含むカード

学習ログ（`data/reviews/*.jsonl`）はこのリポジトリには書き込めません（読み取り専用の公開デモ）。
