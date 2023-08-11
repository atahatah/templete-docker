# templete-docker

これは、自分の Docker 環境の雛形用のレポジトリです。

## コマンド

- Docker Image の構築

```bash
docker-compose build --ssh default --no-cache
```

`--no-cache`はキャッシュを用いたくない場合のみ

- コンテナーを起動

```bash
docker-compose up -d
```

- terminal に入る時

```bash
docker-compose exec -it ubuntu /bin/zsh
```

- 終了

```bash
docker-compose down
```

## 参考

- [Docker で dotfiles のポータビリティーを高める開発環境構築](https://zenn.dev/_kazuya/articles/1c142f23741f15efd169#fn-caa8-1)
- [VSCode Remote Containers を使うなら dotfiles repository で幸せになろう](https://qiita.com/frozenbonito/items/aa320c4b3f84b9816daa)
- [Docker ビルド時にプライベートリポジトリをクローンする](https://zenn.dev/ryo_f/articles/27f223203481ef)
