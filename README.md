## はじめに

HTML を書き換えて見た目を確認したい時、何度もブラウザを手動リロードを繰り返しているとだんだん面倒になってきます。そこで HTML の保存のたびに自動ブラウザのリロードまでやってくれる Live Reload 機能を使いたくなるのですが、npm の live-server というものを使えばそれが実現できます。

## セットアップ

```terminal
npm init -y
npm install live-server
npm set-script start "live-server"

echo "node_modules" > .gitignore

curl https://raw.githubusercontent.com/richardimaoka/html-clone-setup/main/style.css > style.css
curl https://raw.githubusercontent.com/richardimaoka/html-clone-setup/main/index.html > index.html

npm run start
```

後は、以下の動画のように HTML を書き換えながら、保存のたびにブラウザで見た目を確認するだけです。
