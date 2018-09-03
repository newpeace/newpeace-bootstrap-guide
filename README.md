# 対応OS、対応ブラウザ

## 基本方針はOS、ブラウザ共に公式サポートされているもの

## 対応OS
* Windows 7
* Windows 8.1
* Windows 10
* OS X El Capitan 10.11
* macOS Sierra 10.12
* macOS High Sierra 10.13
* iOS 10
* iOS 11
* Android 5.0
* Android 5.1
* Android 6.0
* Android 7.0
* Android 7.1
* Android 8.0

## macOSで対応すべきブラウザ
* Safari 最新版
* Chrome 最新版
* Firefox 最新版

## Windowsで対応すべきブラウザ
* IE 11
* Edge 最新版
* Chrome 最新版
* Firefox 最新版

## iOSで対応すべきブラウザ
* Safari 10
* Safari 11

## Androidで対応すべきブラウザ
* Chrome 最新版


# コーディング要件（スタティックサイトの場合）

## HTML
* HTML5に準拠

## CSS
* CSS3に準拠
* CSSは、Sass(SCSS)もしくはpostCSSをメタ言語として使用
* CSSの基本レイアウトには一般的なフレームワークを使用する
* レスポンシブレイアウトに対応
  * 横幅が320px〜2560pxの間で崩れや横スクロールが起こらず正常に表示できる
  * デバイスの判定は横幅（Media Query）によって行い、UAによって判定しない
  * 少なくともMobile / Tablet (or Small PC) / PC向けに3つのレイアウトと2つのブレイクポイントを持つようにする
* パッケージマネージャーはnpmを使用し、npmを経由しない外部パッケージを追加しない
* リンターはstylelintを使用する

## JavaScript
* ES2015、ES2016、ES2017に準拠
* パッケージマネージャーはnpmを使用し、npmを経由しない外部パッケージを追加しない
* コンパイラーはBabelを使用
* タスクランナーはwebpackもしくはGulpを使用
* リンターはESLintを使用する
  * configは `eslint-config-airbnb-base` を使用する

## プロジェクト
* NEWPEACE Inc.のGitHubリポジトリにてバージョン管理を行う（GitHub Flowに準拠）
* ビルドとテストはCircleCIを使って `master` ブランチが自動的にデプロイされるようにする（セッティングは小川が担当）
* サーバーとして、Amazon S3にホスティングし、CloudFrontをCDNとして用いる（セッティングは小川が担当）
