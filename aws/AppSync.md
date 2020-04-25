# AppSyncのTips

## AppSyncとは

AWSの管理系GraphQLサービス。サーバーレスの形でGraphQLのバックエンドを実装できるサービス

DynamoDB、RDS、Amazon ES (Elasticsearch Service)、Http Endpoint等データソースに直接繋がることもできる。またLambdaと連携することができる

データソースの種類
 - Lambda Function
 - DynamoDB
 - Aurora Serverless （Data API）
 - Elasticsearch Service
 - HTTP
 - None

## 料金

- [AWS AppSync の料金](https://aws.amazon.com/jp/appsync/pricing/)

クエリとデータ変更操作のそれぞれに対し、およびデータのリアルタイム更新に対して個別に請求が発生する。
個人で勉強する際は気にする必要はない。

## 参考URL

- [AWS再入門ブログリレーAppSync編](https://dev.classmethod.jp/articles/relay-re-introduction-2019-appsync/)
- [20190821 AWS Black Belt Online Seminar AWS AppSync](https://www.slideshare.net/AmazonWebServicesJapan/20190821-aws-black-belt-online-seminar-aws-appsync?ref=https://aws.amazon.com/jp/blogs/news/webinar-bb-aws-appsync-2019/)
- [まだAPI Gatewayで消耗してるの？AppSyncのススメ](https://qiita.com/nakayama_cw/items/b7e5db8d25b516440db7)
- [GraphQL入門 (AWS AppSync)](https://www.slideshare.net/AmazonWebServicesJapan/graphql-aws-appsync)