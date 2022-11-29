# analysis_template

## Docker立ち上げ方法

1. `docker compose up -d --build` (イメージ作成→コンテナ作成→コンテナ起動)
2. `docker image ls` (作成されたイメージの確認)
3. `docker container ls` (現在走っているコンテナの確認)
4. `docker compose exec python3 bash` (コンテナへ接続)

- `docker compose down` (コンテナを終了し、削除)
- `docker compose up -d` (コンテナ再起動)
- `docker image rm {imageid}` (イメージ削除)
