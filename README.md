# study-history

## 概要

毎日学んだことをメモするサイトを作る

## 方針

最近勉強したNext.jsを使って作る
-> markdownでblogを作るtutorialがあったのでそのようにしてみる

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
