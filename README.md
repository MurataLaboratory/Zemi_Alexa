# オープンキャンパス用のチャットボット

![test](./img/Github_card.jpg)

# 環境の起動の仕方

dockerで開発したい人は以下のコマンドで環境ができるはず

仮想環境の中にソースがダウンロードされるはず

```
cd alexa_env
docker build -t env .
```

## テストするには

随時更新予定


- ngrokのインストール

```
brew cask intall ngrok
```


# 注意事項

- opensslのばーじょん

仮想環境の中ではどうかわからないけど`openssl version`と打って`LibreSSL`って出るのはだめみたい
