# scraper-line-bot 
※ render version
- LINE Botを使って、入力に応じてwebスクレイピングしてニュース記事を取ってくる
  - 「ヤフーニュース」：トップ5の記事をLINEに表示
  - 「東洋経済オンライン」：トップ5の記事をLINEに表示

# 参考画像
<!-- ![line](https://user-images.githubusercontent.com/34742328/172427140-3546a390-6ae4-4117-a302-4acbeafe6f07.jpg) -->
<img src="https://user-images.githubusercontent.com/34742328/172427140-3546a390-6ae4-4117-a302-4acbeafe6f07.jpg"  width="320px">

# 使い方 WIP
- LINE Developers 登録とかやる
- LINEの公式アカウントを作って、Messaging APIを使えるようにする。
- renderにデプロイして、各種LINEの環境変数の設定をする
  - LINE_CHANNEL_ACCESS_TOKEN、LINE_CHANNEL_SECRET
- Heroku > Setting > BuildPackに以下2つを入れる
  - https://github.com/heroku/heroku-buildpack-chromedriver.git
  - https://github.com/heroku/heroku-buildpack-google-chrome.git
- Messaging APIの設定のWebhookにHeerokuのurl+/callbackを入れる
- Herokuにデプロイする
- Messaging APIで200が返るか確認

# 動作環境
render
