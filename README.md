# modane-live2d-widget

もだねちゃんの Live2D ウィジェット (うごくだけ) です。

## 公開中の URL

GitHub Pages で公開しています。

- [https://modane-live2d-widget.kem198.net](https://modane-live2d-widget.kem198.net)

## 使い方

HTML の `iframe` タグで呼び出して配置します。

```html
<!-- Example -->
<iframe
  id="iframe-modane"
  src="https://kenkenpa198.github.io/modane-live2d-widget/CubismSdkForWeb-4-r.7/Samples/TypeScript/Demo/index.html"
  frameborder="0"
></iframe>
```

表示環境によってはぼやけて表示される問題があります。その場合は下記の Issue を参考にしてください。

- [iframe で表示した際、高解像度ディスプレイでぼやけて表示される](https://github.com/kem198/modane-live2d-widget/issues/1)

## ビルド手順

- [kenkenpa198/practice-live2d-cubism-sdk-for-web](https://github.com/kenkenpa198/practice-live2d-cubism-sdk-for-web)

## 権利表記

### Live2D Cubism SDK for Web について

使用したパッケージや使用許諾に関する情報を掲載しています。

#### 使用したパッケージのバージョン

Cubism 4 SDK for Web R7

- [Live2D Cubism SDK for Web ダウンロード | Live2D Cubism](https://www.live2d.com/sdk/download/web/)

パッケージに含まれる各種ファイルの許諾情報は以降のセクションを参照してください。

#### Live2D Cubism Core について

[Live2D Proprietary Software 使用許諾契約](https://www.live2d.com/eula/live2d-proprietary-software-license-agreement_jp.html) に則り、Live2D Cubism Core は当リポジトリ上で管理・公開していません。

なお GitHub Pages での公開にあたり、当リポジトリでは公式でホスティングされている下記ファイルを参照しています。

- [Live2D Cubism SDK for Web ダウンロード | Live2D Cubism](https://www.live2d.com/sdk/download/web/#url_cubismcore) > `Cubism Core for Web`

ソースの変更箇所は下記のとおりです。

`CubismSdkForWeb-4-r.7/Samples/TypeScript/Demo/index.html`

```html
<head>
  ...
  <!-- <script src = "../../../Core/live2dcubismcore.js"></script> -->
  ★ コメントアウト
  <script src="https://cubism.live2d.com/sdk-web/cubismcore/live2dcubismcore.min.js"></script>
  ★ ホスティング先の URL を記述 ...
  <head></head>
</head>
```

#### Live2D Cubism Components について

[Live2D Open Software 使用許諾契約](https://www.live2d.com/eula/live2d-open-software-license-agreement_jp.html) に則り、下記コンポーネントは当リポジトリ上で管理・公開しています。

- Live2D Cubism Components
  - [Cubism Web Samples](https://github.com/Live2D/CubismWebSamples)
  - [Cubism Web Framework](https://github.com/Live2D/CubismWebFramework)

#### Live2D Cubism サンプルデータについて

[Live2D Cubism サンプルデータ利用条件](https://www.live2d.com/eula/live2d-sample-model-terms_jp.html) に則り、Cubism Web Samples 配下のサンプルデータを当リポジトリで使用しています。

本作品のキャラクターには株式会社Live2Dの著作物であるサンプルデータが株式会社Live2Dの定める規約に従って用いられています。本作品は制作者の完全な自己の裁量で制作されています。
