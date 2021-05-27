# Sauna-Share
<https://app.hiroka-portfolio.com>

自分が行ったおすすめのサウナを写真と一緒に投稿してシェアできるサイトです。
楽天APIを導入してサウナを楽しむためのグッズの検索も可能です。
レスポンシブ対応しているのでスマホからでも利用することができます。
AWSを用いたインフラの構築や、開発環境にdockerとdocker-composeの導入、CircleCIを使ったCI/CDパイプラインGitHubでのissuesでのIssuesとPull requestを活用した擬似チーム開発など、本番を意識して取り組みました。

![トップページ](https://user-images.githubusercontent.com/70800437/119858439-6ef7fe80-bf4f-11eb-85d7-f40af7453599.png)

# 使用技術
- PHP 7.4.15
- Laravel 6.20.26
- MySQL 8.0
- Nginx 1.18.0
- php-fpm
- AWS
  - VPC
  - EC2
  - RDS
  - 画像のアップロードサーバーにS3
  - ACM
  - ELB
  - Route53
- Docker/Docker-compose
- CircleCi CI/CD
- PHPUnit
- 楽天API

# AWS構成図
![aws構成図](https://user-images.githubusercontent.com/70800437/119453408-5d0d3480-bd72-11eb-9dcb-87a1dc7c1215.jpg)

# 機能一覧
- ユーザー登録、ログイン機能
- 記事投稿、削除機能
  - 写真投稿機能(Ajax)
- お気に入り機能
- フォロー機能
- ページネーション機能
- 楽天APIでの商品検索機能

# テスト
- PHPUnit
  - 機能テスト(Feature)
