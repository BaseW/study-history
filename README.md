# study-history

## 概要

毎日学んだことをメモするサイトを作る

## 方針

最近勉強したNext.jsを使って作る
-> markdownでblogを作るtutorialがあったのでそのようにしてみる

- コードスニペットを認識できるようにする
  - [カスタムコンポーネントが必要?](https://goodlife.tech/posts/react-markdown-code-highlight.html)
- 日付などで絞り込み
  - 10件ごと
  - 入力して検索
- 選択したキーワードをタグにしたり、そのタグから検索できるようにしたい
  - MeCabで形態素解析して選択?
  - 自由選択?
- S3にmarkdownをアップロード?
  - [S3をnode.jsから使う方法](https://docs.aws.amazon.com/ja_jp/sdk-for-javascript/v2/developer-guide/s3-example-creating-buckets.html)
  - `@aws-sdk/client-s3`を使う?
- どのくらい活動しているかを可視化する(githubのように)
  - [FullCalendar](https://qiita.com/yk2220s/items/8ed4d781412f6c4e9c45)


