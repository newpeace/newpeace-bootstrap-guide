# 対応OS、対応ブラウザ

## 基本方針はOS、ブラウザ共に公式サポートされているもの

## 対応OS
* Windows Vista, 7, 8.1, 10
* macOS 10.9, 10.10, 10.11, 10.12
* iOS 7, 8, 9, 10
* Android 4.4, 5.0, 5.1, 6.0, 7.0

## macOS
* Safari 7, 8, 9, 10
* Chrome 最新版
* Firefox 最新版

## Windows
* IE 9, 10, 11
* Edge 最新版
* Chrome 最新版
* Firefox 最新版

## iOS
* Safari 7, 8, 9, 10

## Android
* Chrome 最新版
* 標準ブラウザ（例外的にAndroid 4.0以降に対応）


# コーディング要件
* Jekyllを静的サイトジェネレーターとして使用
* CSSは、Sass(SCSS)もしくはpostCSSをメタ言語として使用
* JSは、ES2015およびES2016に準拠し、AltJSを用いる場合は、TypeScriptを使用
* コンパイラーはBabelを使用
* タスクランナーはwebpackもしくはGulpを使用
* CSSフレームワークとして、Bootstrapを使用、それ以外を使う場合は応相談
* レスポンシブレイアウトに対応し、どのような横幅のデバイスで見ても崩れや横スクロールが起こらないようにし、デバイスの判定は横幅によって行って、少なくともMobile / Tablet / PC向けに3つのレイアウトと2つのブレイクポイントを持つようにする。
* NEWPEACE Inc.のGitHubリポジトリにてバージョン管理を行う（GitHub Flowに準拠）
* ビルドとテストはCircleCIを使って `master` ブランチが自動的にデプロイされるようにする（セッティングは小川が担当）
* サーバーとして、Amazon S3にホスティングし、CloudFrontをCDNとして用いる（セッティングは小川が担当）
