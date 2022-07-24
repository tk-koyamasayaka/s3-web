# s3-web

S3を使用したコンテンツ配信を試してみるのが目的であるため、デザインは最低限のものになっています。

## Infrastructure

* AWS S3
* Route53
* Cloudfront
  * AWS Certificate ManagerでSSL証明書を発行しています。

## Deploy

* [Github Actions](https://github.com/wannyanland/s3-web/blob/master/.github/workflows/deploy.yml)で自動デプロイ環境を構築しています。
* masterブランチへのプッシュイベントをトリガーにS3へデプロイしています。
* ビルドが不要なため非常にシンプルな記述になっています。

