# 職務経歴書
最終更新日: {docsify-updated} 

## 基本情報
|key|value|
|---|---|
|氏名|高橋大地 (Takahashi, Daichi)|
|生年月|1991年6月|
|居住地|東京都|
|最終学歴|筑波大学大学院 人間総合科学研究科 芸術専攻 修了（修士デザイン学）|
|GitHub|https://github.com/daichitakahashi|
|Zenn|https://zenn.dev/daichitakahashi|

主にバックエンドエンジニアとして経験を積んでおり、パフォーマンスや信頼性を重視した開発を志向しています。
これを実現するために、テスト容易性やテストの信頼性を向上させるためのコード設計や環境整備にも積極的に取り組んできました。

研究室助手としての業務では、学生、研究室スタッフ、教員、外部講師、事務職員など、さまざまな関係者のなかで調整を行いながら業務を進行させる経験を積みました。

2023年10月よりフルスタックエンジニアとして設計から開発、運用を担うようになり、総合的にスキルを向上させていくことで、企業の目的達成のために活躍できるエンジニアを目指しています。

## スキル
### 得意とする開発言語
- Go
  - 主な使用言語として5年ほどの経験
  - ゼロベースでのAPIサーバーの構築
  - 並行処理やストリーム処理を活用し、パフォーマンスを意識した実装を行うことができる
  - AST操作を用いたコード生成ツールの作成
- JavaScript
- TypeScript
  - フロントエンド開発のほか、Cloudflare Workersを使用したフルスタックな開発に使用

### フレームワーク/ライブラリ
- [99designs/gqlgen](https://github.com/99designs/gqlgen)
- [sqlc-dev/sqlc](https://github.com/sqlc-dev/sqlc)
- [labstack/echo](https://github.com/labstack/echo)
- [gin-gonic/gin](https://github.com/gin-gonic/gin)
- [connectrpc/connect-go](https://github.com/connectrpc/connect-go)
- [golangci/golangci-lint](https://github.com/golangci/golangci-lint)
- [React](https://github.com/facebook/react)
- [Remix](https://github.com/remix-run/remix)
- [Hono](https://github.com/honojs/hono)
- [Drizzle](https://github.com/drizzle-team/drizzle-orm)
- [Pulumi](https://github.com/pulumi/pulumi)
- [Biome](https://github.com/biomejs/biome)
- [Playwright](https://github.com/microsoft/playwright)

### データストア
- MySQL
- PostgreSQL
- SQLite3
- Redis

### 通信プロトコル
- GraphQL
- REST
- gRPC

スキーマファーストなAPI設計/実装を得意としている。

### PaaS, BaaS
- AWS
  - 業務ではECS Fargate、LambdaやAurora(MySQL), ElastiCache(Redis), OpenSearch Service等を使用
- Cloudflare
  - Cloudflare Workers, Cloudflare Pagesを活用して社内用アプリケーションを構築
  - Cloudflare Zero Trustを活用した社内システムの保護
- supabase

### その他ツール
- Docker
  - アプリケーション開発の他に、テスト環境の整備の一環としてコンテナイメージ開発を行う
- GitLab
  - 業務で使用
  - 社内でホストしたCIランナーの運用、保守
  - CI/CDパイプラインの設計、構築
- GitHub
  - 業務、個人開発で使用
  - CI/CDパイプラインの設計、構築
- [VitePress](https://github.com/vuejs/vitepress)
  - 社内用ドキュメントの管理
- [k1LoW/tbls](https://github.com/k1LoW/tbls)
  - データベースからのER図生成

---

## 職務経歴
### コウソミル株式会社(2024年10月〜)
*システムエンジニア*

疾患の早期診断薬を開発するスタートアップに、検査体制を支える社内システムを開発する1人目のエンジニアとして参加。

#### <u>検査追跡システム開発(2024年10月〜)</u>
- **プロジェクトの規模**
  - 7名（エンジニア1名、検査チーム6名）
- **プロジェクト詳細**
  - 受注した検査の適切な進行を補助し、記録を追跡可能にするためのシステム
  - 提携企業とのAPI連携
- **役割**
  - 検査チームからのヒアリング、要件定義
  - システム設計
    - Cloudflare PagesとCloudflare Workersを使用
    - Cloudflare Workersはサービス単位で開発
      - プロジェクト管理サービス、受注サービス、検査進行管理サービス、在庫管理サービス
    - Cloudflare Zero Trustによるアクセス制限
  - Figmaを使用した画面設計
  - コードファーストでのテーブル設計
    - supabaseが提供するPostgreSQLを使用
    - サービス単位でのDB分割
    - tblsを使用したER図の自動生成
  - ER図やシステム関連図等各種ドキュメントの作成、管理
  - CI/CDパイプラインの設計
    - GitHub Actions
    - IaCとしてPulumiを採用
  - 開発
    - バックエンド: TypeScript, Hono
    - フロントエンド: TypeScript, Remix
  - 今後の業務
    - テスト
    - 運用、監視
    - API連携に関する提携企業との調整

### 株式会社クオリティア(2020年4月〜2023年9月)
*クラウドサービス本部 開発部 主任*

バックエンドエンジニアとしてSaaS型のWebメール製品と認証基盤製品の開発に従事。
APIの設計、開発に取り組むほか、脆弱性やパフォーマンス上の課題の発見とその改善にも積極的に取り組む。

#### <u>Webメール製品開発(2020年4月〜)</u>
- **プロジェクトの規模**
  - 7名（バックエンドエンジニア2名）
- **プロジェクト詳細**
  - SaaS型のメール製品
  - ユーザーによるメール操作機能のほか、ドメインやユーザー管理機能、監査機能をもつ
  - バックエンドはGo, フロントエンドはTypeScript+Reactで開発
- **役割**
  - API設計(GraphQL, REST, gRPC)、実装
    - アプリケーションはコンテナとしてAmazon ECSにデプロイ
  - 受信メールのサニタイズ、メール作成、送信等のコア機能の開発
    - パフォーマンス改善に大きく貢献
  - RDBのテーブル設計
  - Redisを用いた分散環境下での排他制御の実装
  - CI/CDパイプラインの設計/実装
    - GitLab CI
  - TypeScript+ReactでのSPA開発のサポート
  - 品質管理部によるE2Eテストプロジェクトのサポート（Playwright）
  - 再設計に伴い、モジュラモノリスの導入
  - ユニットテスト作成のリード

#### <u>認証基盤製品開発（2021年10月〜2022年8月）</u>
- **プロジェクトの規模**
  - 6名（バックエンドエンジニア2名）
- **プロジェクト詳細**
  - SaaS型の認証基盤
  - 専用のブラウザアプリを通じたシングルサインオン機能を提供
- **役割**
  - 仕様検討
  - API設計(GraphQL, REST)、実装
    - アプリケーションはコンテナとしてAmazon ECSにデプロイ
  - RDBのテーブル設計
  - ソフトウェアアーキテクチャの設計
  - Redisを用いた分散環境下での排他制御の実装
  - Goの共通ライブラリの開発、メンテナンス
  - コード生成を使用した開発支援ツールの開発、メンテナンス
  - ユニットテスト作成のリード
  - オフショア開発者との調整

### 学校法人武蔵野美術大学（2016年4月〜2020年3月）
*デザイン情報学科研究室 助手*

研究室及び学科運営（講義、演習の管理/運営、学生の指導、経理、機器備品管理等々…）の傍ら、学生の成果展示の計画を支援するシステムを開発。

#### <u>備品貸し出し申請フォーム＋集計フォームの開発</u>
- **プロジェクトの規模**
  - 1名
- **プロジェクト詳細**
  - 100人超の学生が一堂に会する作品展示のための備品貸し出しや消費電力量の管理を行うためのCGIを開発
- **役割**
  - 仕様検討
  - 設計
  - 開発

---

## 業務外での活動
### OSS開発
-  daichitakahashi/confort
  - https://github.com/daichitakahashi/confort
  - コンテナを使用した並列テストのためのテストヘルパー(Go)
  - 紹介記事
    - https://zenn.dev/daichitakahashi/articles/9e091863f158b7
- daichitakahashi/rsmap
  - https://github.com/daichitakahashi/rsmap
  - 並列テストにおけるプロセス外のリソース使用の排他制御を行うテストヘルパー(Go)
  - confortの後継として開発中
