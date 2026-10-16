# ILLUSIONARY — Prompt Archive

Y2K / cybercore / electric-blue graphic style with pixel-inspired typographyの、GitHub Pages向けプロンプト保管サイトです。データベースやサーバーは不要です。

## ファイル構成

- `index.html` — トップページとキャラクター一覧
- `style.css` — 全ページのデザイン
- `characters.json` — 一覧に表示する名前・画像・詳細ページ
- `characters/character-001.html` — 詳細ページのテンプレート
- `images/` — キャラクター画像を入れるフォルダ

## GitHub Pagesで公開

1. GitHubでPublicリポジトリを作成
2. ZIPを解凍し、中にあるファイルとフォルダをリポジトリの一番上にアップロード
3. リポジトリの **Settings → Pages** を開く
4. **Deploy from a branch** を選び、`main` と `/(root)` を指定して保存

## キャラクター画像を入れる

画像を `images` フォルダに入れ、次の名前にしてください。

- `character-001.jpg`
- `character-002.jpg`

PNG画像なら、HTMLと`characters.json`の拡張子も `.png` に変更します。

## キャラクターを追加する

1. `characters/character-001.html`を複製し、ファイル名を `character-003.html` などにする
2. ページ内の名前・番号・画像パス・プロンプトを書き換える
3. `characters.json` の配列に1件追加する。例：

```json
{
  "name": "Character Name 003",
  "image": "images/character-003.jpg",
  "page": "characters/character-003.html"
}
```

## メモ

- 名前やプロンプトはサンプルです。公開前に自分の内容へ変更してください。
- 画像ファイル自体はサンプルに含めていません。
- コピー機能はボタン1回で動作します。ブラウザの制限時は代替コピー処理を試します。
- Google Fontsが利用できない環境では、端末の標準フォントで表示されます。
