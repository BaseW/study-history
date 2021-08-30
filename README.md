# study-history

## 概要

毎日学んだことをメモするサイトを作る

## 方針

最近勉強したNext.jsを使って作る
-> markdownでblogを作るtutorialがあったのでそのようにしてみる

選択したキーワードをタグにしたり、そのタグから検索できるようにしたい

This is a starter template for [Learn Next.js](https://nextjs.org/learn).

## メモ

ある程度形になるまでメモしておく
ひとまず[チュートリアル](https://nextjs.org/learn/basics/create-nextjs-app?utm_source=next-site&utm_medium=homepage-cta&utm_campaign=next-website)に沿っていく

- 2021/08/26
  - sedを直接リダイレクトしようとするとファイルが初期化されてしまうので注意
  - (pytestで)同じDBに書き込んでから最新のレコードを読み込むと順番が前後した
  - macでword skipは command + right arrow
  - macのvscodeで定義参照 -> 戻るには ctrl + -
  - Next.jsのLinkコンポーネントを使うと、clientでページ遷移できる
- 2021/08/27
  - Next.jsのImageコンポーネントは最適化を行う(public/images/~.jpg)
  - Next.jsのHeadコンポーネントでタイトルをつけられる
  - Next.jsでは`styled-jsx`によって、Reactコンポーネント内でcssを書ける
  - Layoutコンポーネントにcssを当てるにはCss Modulesを使う(components/layout(.js/.module.css))
  - Css Modulesは自動で一意なclassNameを生成する
  - 全体にcssを反映するためにはpages/_app.jsを使う(styles/global.css)
  - app.diagrams.netで図を作成できる https://qiita.com/cloudsnow/items/77e591d63dd7117d3380
  - Next.jsはデフォルトでpre-renderingを行う
  - pre-renderingはSEOに効果的
  - 生のreact.jsはpre-renderingしていない
  - Next.jsのpre-renderingには2種類ある
    - Static Generation
    - Server-side Rendering
  - Static Generationでもデータを取得できる -> `getStaticProps`
  - [gray-matter](https://github.com/jonschlinkert/gray-matter)はmarkdownのmetadataを解析する
  - `getStaticProps`でpropsを返し、`Home`コンポーネントで受け取る
  - `getStaticProps`でAPIやDBにもアクセス可能
  - Server-side Renderingの場合は`getServerSideProps`を使う
- 2021/08/30
  - -> と return でシーケンス図が描ける
  - fastapiのrouterの関数のコメントはdocsにも表示される
  - markdown(git)の中で相対パスによるリンクを書ける
- 2021/08/31
  - Next.jsの動的ルーティングは`pages/[id].js`のようなファイルで行う
  - `[id].js`は""で囲うことで作成できる(\でも可能だった)
  - remarkでmarkdownをhtmlとして解析できる
  - date-fnsで時刻をフォーマット
  - getStaticPropsで`fallback: false`とすると、取得失敗時に404を返す
  - ネストしたルートも取得できる
  - `pages/api`内でhandlerを定義するとAPI Routeを定義できる
  - `getStaticProps`と`getStaticPaths`はサーバーサイドでのみ実行される
  - Vercelを使ってNext.jsアプリをデプロイできる
  - プルリクを作成すると、previewできる
  - DPS(Develop, Previwe, Ship)のワークフロー
