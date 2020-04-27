# GraphQLのTips

## スキーマ

APIの仕様を表現するもの。キーマ定義言語（SDL(Schema Definition Language)）を使って表現する。

一般的、拡張子は`graphqls`となる。

[GraphQLのスキーマと型定義](https://qiita.com/NagaokaKenichi/items/d341dc092012e05d6606)


inputは引数の型?みたいなのを定義する

```
input MessageInput {
  content: String
  author: String
}

type Mutation {
  createMessage(input: MessageInput): Message
  updateMessage(id: ID!, input: MessageInput): Message
}
```

## リゾルバ

ひとつひとつのフィールドはリゾルバ（resolver）と呼ばれる関数がマッピングされます。リゾルバは、オブジェクト（例えばUserのインスタンス）を引数として受け取り、そのオブジェクトのプロパティ（例えばUser#name）を返すシンプルな関数です。

データソースとマッピングを行う

## GitHubのGraphQLを叩く

- [GitHub GraphQL API](https://developer.github.com/v4/explorer/)
- [公式リファレンス](https://developer.github.com/v4/explorer/)

## 参考URL

- [GraphQLのクエリを基礎から整理してみた](https://qiita.com/shunp/items/d85fc47b33e1b3a88167)
- [Web API初心者と学ぶGraphQL](https://qiita.com/SiragumoHuin/items/cc58f456bc43a1be41b4)