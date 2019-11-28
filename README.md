# SwaggerのYamlを分割してRedocで静的ファイルを作成するサンプル

## 実行サンプル

サンプルのYAMLは公式のPetStore

### 分割したファイルのマージ

```
npm run merge
```

### マージしたYAMLからHTMLを作成

```
npm run html
```

### マージ〜HTMLを一回で

```
npm run make
```

### 修正しながらmakeしてブラウザで確認したい場合

```
npm run dev
```

## 作り方

```
npm install --save-dev redoc-cli
npm install --save-dev swagger-merger
npm install --save-dev npm-run-all
npm install --save-dev watch
npm install --save-dev light-server

分割とHTMLだけなら最初の2つだけあればOK

残りはsrc配下のファイルを監視して更新があったら
ビルドして、htmlが新しくなったらオートリロードさせてブラウザ側に
反映させる感じの事に使用。
```

