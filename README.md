# analysis_template

## Docker立ち上げ方法

1. `docker compose up -d --build` (イメージ作成→コンテナ作成→コンテナ起動)
2. `docker image ls` (作成されたイメージの確認)
3. `docker container ls` (現在走っているコンテナの確認)
4. `docker compose exec python3 bash` (コンテナへ接続)

- `docker compose down` (コンテナを終了し、削除)
- `docker compose up -d` (コンテナ再起動)
- `docker image rm {imageid}` (イメージ削除)
- `docker run -v $PWD/opt:/root/opt -w /root/opt -it --rm -p 7777:8888 docker-python-python3 jupyter-lab --ip 0.0.0.0 --allow-root -b localhost` (Jupyter Notebook立ち上げ)　<http://127.0.0.1:7777>

## ディレクトリ構成

- input (train.csv, test.csvなどの入力ファイルを入れるフォルダ)
- code (計算用のコードのフォルダ)
- code-analysis (分析用のコードやJupyter Notebookのフォルダ)
- model (モデルや特徴量を保存するフォルダ)
- submission (提出用ファイルを保存するフォルダ)
