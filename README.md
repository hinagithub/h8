

## リポジトリの説明
「12ステップで作る 組込みOS自作入門」の実装に必要なソースや手順を置いている

## 参考本・サポートページ
[12ステップで作る 組込みOS自作入門](http://kozos.jp/books/makeos/)
[Docker file gcc3/h8300/](https://github.com/srz-zumix/gcc3/tree/master/h8300)

## オリジナルソース
[「12ステップで作る 組込みＯＳ自作入門」のソースコード](https://kozos.jp/kozos/osbook/osbook_03/)

##　Macで環境構築するための手順メモ
　[【C】 cozosOSを触るにあたり調べたこと](https://hinahinako.github.io/mypage/2022/03/19/C-cozosOS%E3%82%92%E8%A7%A6%E3%82%8B%E3%81%AB%E3%81%82%E3%81%9F%E3%82%8A%E8%AA%BF%E3%81%B9%E3%81%9F%E3%81%93%E3%81%A8.html)

## Docker起動方法
```
docker compose build ubuntu-h8
docker compose up -d
docker ps

>
---------------------------------------------------------------------------------------------------------------------------------------------------
CONTAINER ID   IMAGE              COMMAND   CREATED          STATUS          PORTS                  NAMES
container-id-xxx   osbook_ubuntu-h8   "bash"    27 seconds ago   Up 27 seconds   0.0.0.0:5001->80/tcp   osbook-ubuntu-h8-service-1
---------------------------------------------------------------------------------------------------------------------------------------------------
```

bash
```
docker exec -it container-id-xxx bash
```

ポイント
- `make image` はDocker上で実行。
- `make write` はローカルで実行。



