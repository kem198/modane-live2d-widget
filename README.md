<!-- omit in toc -->
# modane-live2d-widget

もだねちゃんの Live2D パーツです。

<!-- omit in toc -->
## 目次

- [1. Live2D Cubism SDK for Web について](#1-live2d-cubism-sdk-for-web-について)
    - [1.1. 使用したパッケージのバージョン](#11-使用したパッケージのバージョン)
    - [1.2. Live2D Cubism Core について](#12-live2d-cubism-core-について)
    - [1.3. Live2D Cubism Components について](#13-live2d-cubism-components-について)
    - [1.4. Live2D Cubism サンプルデータについて](#14-live2d-cubism-サンプルデータについて)
    - [1.5. コアの外部読み込み](#15-コアの外部読み込み)
- [2. ビルド手順](#2-ビルド手順)

## 1. Live2D Cubism SDK for Web について

使用したパッケージや使用許諾に関する情報を掲載しています。

### 1.1. 使用したパッケージのバージョン

Cubism 4 SDK for Web R7

- [Live2D Cubism SDK for Web ダウンロード | Live2D Cubism](https://www.live2d.com/sdk/download/web/)

パッケージに含まれる各種ファイルの許諾情報は以降のセクションを参照してください。

### 1.2. Live2D Cubism Core について

[Live2D Proprietary Software 使用許諾契約](https://www.live2d.com/eula/live2d-proprietary-software-license-agreement_jp.html) に則り、Live2D Cubism Core は当リポジトリ上で管理・公開していません。Cubism Core は Cubism SDK 配布パッケージに同梱されているので、別途ダウンロードしてください。

なお GitHub Pages での公開にあたり、当リポジトリでは公式でホスティングされている下記ファイルを参照しています。

- [Live2D Cubism SDK for Web ダウンロード | Live2D Cubism](https://www.live2d.com/sdk/download/web/#url_cubismcore) > `Cubism Core for Web`

ソースの変更箇所は下記のとおりです。

`CubismSdkForWeb-4-r.7/Samples/TypeScript/Demo/index.html`

```html
<head>
  ...
  <!-- <script src = "../../../Core/live2dcubismcore.js"></script> -->                         ★ コメントアウト
  <script src="https://cubism.live2d.com/sdk-web/cubismcore/live2dcubismcore.min.js"></script> ★ ホスティング先の URL を記述
  ...
<head>
```

### 1.3. Live2D Cubism Components について

[Live2D Open Software 使用許諾契約](https://www.live2d.com/eula/live2d-open-software-license-agreement_jp.html) に則り、下記コンポーネントは当リポジトリ上で管理・公開しています。

- Live2D Cubism Components
    - [Cubism Web Samples](https://github.com/Live2D/CubismWebSamples)
    - [Cubism Web Framework](https://github.com/Live2D/CubismWebFramework)

### 1.4. Live2D Cubism サンプルデータについて

[Live2D Cubism サンプルデータ利用条件](https://www.live2d.com/eula/live2d-sample-model-terms_jp.html) に則り、Cubism Web Samples 配下のサンプルデータを当リポジトリで使用しています。

本作品のキャラクターには株式会社Live2Dの著作物であるサンプルデータが株式会社Live2Dの定める規約に従って用いられています。本作品は制作者の完全な自己の裁量で制作されています。

### 1.5. コアの外部読み込み

当リポジトリの `Cubism 4 SDK for Web R7` 配下のサンプルファイルについて、オリジナルから記述を一部更新しています。

`CubismSdkForWeb-4-r.7/Samples/TypeScript/Demo/index.html`

```html
<head>
  ...
  <!-- <script src = "../../../Core/live2dcubismcore.js"></script> -->                         ★ コメントアウト
  <script src="https://cubism.live2d.com/sdk-web/cubismcore/live2dcubismcore.min.js"></script> ★ ホスティング先の URL を記述
  ...
<head>
```

Live2D Cubism Core の再頒布・公開は前述の規約により禁止されているので、GitHub リポジトリ上に配置できません。そのため公式でホスティングされている下記ファイルを参照しています。

- [Live2D Cubism SDK for Web ダウンロード | Live2D Cubism](https://www.live2d.com/sdk/download/web/#url_cubismcore) > `Cubism Core for Web`

## 2. ビルド手順

- [kenkenpa198/practice-live2d-cubism-sdk-for-web](https://github.com/kenkenpa198/practice-live2d-cubism-sdk-for-web)
