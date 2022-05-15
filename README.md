# Docker上で環境構築をしたRails tutorialのアプリケーション
dir名 : sample-app-latest

これは、次の教材で作られたサンプルアプリケーションです。
[*Ruby on Rails チュートリアル*](https://railstutorial.jp/)
（第6版）
[Michael Hartl](https://www.michaelhartl.com/) 著

## ライセンス

[Ruby on Rails チュートリアル](https://railstutorial.jp/)内にある
ソースコードはMITライセンスとBeerwareライセンスのもとで公開されています。
詳細は [LICENSE.md](LICENSE.md) をご覧ください。

## 使い方

このアプリケーションを動かす場合は、Docker が PC　に setup されている必要があります。
以下のコマンドで、build して、 container を起動します。

```
$ docker-compose up --build
```

localhost のport　番号 3000　にアクセスします。


データベースへのマイグレーションを実行、あるいは bundle install する場合は、 container 上で行う必要があるので、以下のコマンドを実行し、 container 内に入ります。

```
$ docker-compose exec web bash
```
