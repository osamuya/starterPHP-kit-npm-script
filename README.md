# starter-kit(npm-script)
npm-scriptを使ったフロントエンド開発環境

## 2017.11.19(sun)

開発途中

## 2017.11.26(sun)

- node sassからpostcssに変更
- windows環境でも使用できるようにnpm-run-allをinstall
- css:FLOCSSに変更


# usage

node_moduleのインストール
````
npm install
````
starter-kitの起動
````
npm run start
````

## PHPを使う場合

あらかじめPHPの起動する環境を作成します。

- Virtualhostの作成 (XAMPPとかMAMPPとかLinuxサーバーとかで)
- (例)ホスト: sample.localhost
- package.jsonの10行目のproxyを該当のホストに変更

````
browser-sync start --proxy sample.localhost --port 3000 ...
````

## PHPを使わない場合

- Virtualhostの作成はしなくていいです。
- package.jsonの10行目を--serverオプションでもって相対パスでDocumentRootを指定します。

````
browser-sync start --server ./public/ --port 3000 ...
````





