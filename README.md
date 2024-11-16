# trend-watcher

## Vite + Vue + TypeScript

インストール
```
docker compose run --rm app npm ci
```

起動
```
docker compose up -d
```

以下にアクセス
```
http://localhost:5173
```

コンテナ、イメージ、ネットワーク、ボリューム、キャッシュの削除
```
docker stop $(docker ps -aq) && docker rm $(docker ps -aq) && docker rmi -f $(docker images -aq) && docker network prune -f && docker volume prune -f && docker builder prune -a -f
```
