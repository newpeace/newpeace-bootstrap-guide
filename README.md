# 対応OS、対応ブラウザ

## 基本方針はOS、ブラウザ共に公式サポートされているもの

## 対応OS
* Windows 7
* Windows 8.1
* Windows 10
* OS X Yosemite 10.10
* OS X El Capitan 10.11
* macOS Sierra 10.12
* iOS 8
* iOS 9
* iOS 10
* Android 4.4
* Android 5.0
* Android 5.1
* Android 6.0
* Android 7.0
* Android 7.1

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
* Safari 8
* Safari 9
* Safari 10

## Androidで対応すべきブラウザ
* Chrome 最新版
* 標準ブラウザ（例外的にAndroid 4.1以降に対応）


# コーディング要件

## HTML
* Jekyllを静的サイトジェネレーターとして使用

## CSS
* CSSは、Sass(SCSS)もしくはpostCSSをメタ言語として使用
* CSSフレームワークとして、Bootstrapを使用、それ以外を使う場合は応相談
* レスポンシブレイアウトに対応し、どのような横幅のデバイスで見ても崩れや横スクロールが起こらないようにし、デバイスの判定は横幅によって行って、少なくともMobile / Tablet / PC向けに3つのレイアウトと2つのブレイクポイントを持つようにする。

## JavaScript
* JSは、ES2015およびES2016に準拠し、AltJSを用いる場合は、TypeScriptを使用
* コンパイラーはBabelを使用
* タスクランナーはwebpackもしくはGulpを使用

## プロジェクト
* NEWPEACE Inc.のGitHubリポジトリにてバージョン管理を行う（GitHub Flowに準拠）
* ビルドとテストはCircleCIを使って `master` ブランチが自動的にデプロイされるようにする（セッティングは小川が担当）
* サーバーとして、Amazon S3にホスティングし、CloudFrontをCDNとして用いる（セッティングは小川が担当）
