# amplifyのTips

## amplifyとは

Webやモバイル向けのAWSサービスを簡単に構築できるサービス

[AWS Amplifyとはなんなのか３行で表現する](https://qiita.com/laha/items/1e0805edacce111e9332)

## Amplify CLI

対話形式でAWSのサービスでモバイルアプリケーションのバックエンドとしてよく使われるサーバーレス構成を自動でセットアップできる

### amplify init

プロジェクトの初期化を行う。ローカルとAWSを紐付ける。

```
👉  amplify-webapp (master) $ amplify init
Note: It is recommended to run this command from the root of your app directory
? Enter a name for the project amplifywebapp
? Enter a name for the environment dev
? Choose your default editor: Visual Studio Code
? Choose the type of app that you're building javascript
Please tell us about your project
? What javascript framework are you using vue
? Source Directory Path:  src
? Distribution Directory Path: dist
? Build Command:  yarn build
? Start Command: yarn serve
Using default provider  awscloudformation

For more information on AWS Profiles, see:
https://docs.aws.amazon.com/cli/latest/userguide/cli-multiple-profiles.html

? Do you want to use an AWS profile? Yes
? Please choose the profile you want to use default
Adding backend environment dev to AWS Amplify Console app: d1vl0gqabn3bh0
```

### amplify add

アプリケーションにAmplifyの用意している機能を追加する。

```
👉  amplify-webapp (master *%) $ amplify add api
? Please select from one of the below mentioned services: GraphQL? Provide API name: amplifywebapp
? Choose the default authorization type for the API API key
? Enter a description for the API key: for Amplify Web App
? After how many days from now the API key should expire (1-365): 7
? Do you want to configure advanced settings for the GraphQL API No, I am done.
? Do you have an annotated GraphQL schema? No
? Do you want a guided schema creation? Yes
? What best describes your project: Single object with fields (e.g., “Todo” with ID, name, description)
? Do you want to edit the schema now? Yes
Please edit the file in your editor: /Users/suzuki_naoto/private_project/amplify-webapp/amplify/backend/api/amplifywebapp/schema.graphql
? Press enter to continue 
```

### amplify push

```
👉  amplify-webapp (master *%) $ amplify push✔ Successfully pulled backend environment dev from the cloud.

Current Environment: dev

| Category | Resource name | Operation | Provider plugin   |
| -------- | ------------- | --------- | ----------------- |
| Api      | amplifywebapp | Create    | awscloudformation |
? Are you sure you want to continue? Yes

The following types do not have '@auth' enabled. Consider using @auth with @model
         - City
Learn more about @auth here: https://aws-amplify.github.io/docs/cli-toolchain/graphql#auth 


GraphQL schema compiled successfully.

Edit your schema at /Users/suzuki_naoto/private_project/amplify-webapp/amplify/backend/api/amplifywebapp/schema.graphql or place .graphql files in a directory at /Users/suzuki_naoto/private_project/amplify-webapp/amplify/backend/api/amplifywebapp/schema
? Do you want to generate code for your newly created GraphQL API Yes
? Choose the code generation language target typescript
? Enter the file name pattern of graphql queries, mutations and subscriptions src/graphql/**/*.ts
? Do you want to generate/update all possible GraphQL operations - queries, mutations and subscriptions Yes
? Enter maximum statement depth [increase from default if your schema is deeply nested] 2
? Enter the file name for the generated code src/API.ts
⠴ Updating resources in the cloud. This may take a few minutes...
```