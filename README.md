# GradleSandbox [![Build Status](https://travis-ci.org/ichigotake/GradleSandbox.png)](https://travis-ci.org/ichigotake/GradleSandbox)

## 概要

自分のAndroidのビルド環境(主に`build.gradle`)をチートシートとして利用出来るようにまとめたもの

## 内容

`build.gradle` と [コミットログ](https://github.com/ichigotake/AndroidBuildSettingExample/commits/master) を参照

- `generateManifest` BuildVariants毎のAndroidManifest.xmlを用意するカスタムタスク
- [gfx/android-gradle-utils](https://github.com/gfx/gradle-android-utils) を利用
    - local.propertiesが存在しない場合に自動生成する
    - デバッグビルド時にアプリアイコンをグレースケールにする
    - バージョン更新をバージョン名のみで対応(バージョンコードは自動生成される
- BuildConfigFieldを利用して定数を `BuildConfid` へセットする
- Gradleで署名ビルド
- travis-ciでDalvikVMを利用したテストを実行
- ライブラリプロジェクトのmavenレポジトリをgitレポジトリに内包
- 端末内に複数のBuildVariantsを共存させる

