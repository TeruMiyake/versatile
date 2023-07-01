# Dockerfile のリファレンスとベスト・プラクティス
# https://docs.docker.jp/engine/reference/builder.html
# https://docs.docker.jp/develop/develop-images/dockerfile_best-practices.html

# Dockerfile の基本的なテンプレート
# https://docs.docker.jp/engine/reference/builder.html

# ベースイメージの指定
FROM node:lts-hydrogen

# vim インストール
RUN apt-get update && apt-get install -y \
    vim \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# コンテナのユーザを変更
USER node

# ワークディレクトリの指定（以降の RUN 命令等の作業ディレクトリを指定）
RUN mkdir -p /home/node/versatile
WORKDIR /home/node/versatile