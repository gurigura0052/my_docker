## コンテナを作成して、起動
```
$ docker-compose up -d
```

## 既にコンテナがある状態でサービスを開始
```
$ docker-compose start
```

## サービスを停止
```
$ docker-compose stop
```

## コンテナを停止し、コンテナとネットワークを削除
```
$ docker-compose down
```

## コンテナの中で作業を開始
```
$ docker-compose exec web /bin/bash

$ docker-compose exec db /bin/bash
```

## 全てのコンテナ・イメージを削除
### 全てのコンテナを停止
```
$ docker stop $(docker ps -q)
```

### 全てのコンテナを削除
```
$ docker rm $(docker ps -q -a)
```

### 全てのイマージを削除
```
$ docker rmi $(docker images -q) -f
```