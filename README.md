# Docker上で環境構築をしたrailsのbase container 
#### rails で開発する際に使用を想定
#### bootstrap はまだ動かないので、修正中。

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
