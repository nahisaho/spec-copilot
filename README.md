# Spec Copilot - Interactive agent to support specification-driven development

> **仕様駆動開発を支援するための対話型エージェント**
>
> GitHub Copilot で仕様駆動開発を支援するための対話型エージェント群です。

---

## 📖 概要

このディレクトリには、ソフトウェア開発のあらゆる局面をサポートする**19種類の専門AIエージェント**のプロンプトが含まれています。各エージェントは特定のドメインに特化し、段階的な対話フローと実践的なガイドラインを提供します。

### 🎯 特徴

- ✅ **専門特化型**: 各エージェントが特定の技術領域に特化
- ✅ **構造化された対話フロー**: 1問1答形式で段階的に情報を収集
- ✅ **実践的なコード例**: すぐに使える実装例とベストプラクティス
- ✅ **ファイル出力対応**: 設計書・仕様書・テストコードを自動生成
- ✅ **包括的なフレームワーク**: 業界標準の手法とツールを網羅
- ✅ **アクセシビリティ重視**: WCAG準拠やセキュリティ対応を標準装備

---

## 🤖 エージェント一覧

### 1. 🎭 **Orchestrator AI**
**ファイル**: `orchestrator.md`

マルチエージェントシステムのオーケストレーター。ユーザーのリクエストを分析し、最適なエージェントを選択・連携させます。

**主な機能**:
- リクエスト分析とエージェント選定
- 複数エージェントの並列・順次実行
- タスク分解と依存関係管理
- 実行計画の最適化

**使用場面**: 複雑なプロジェクトで複数の専門領域が必要な場合

---

### 2. 🏃 **Agile Coach AI**
**ファイル**: `agile-coach.md`

アジャイル開発のベストプラクティスを提供するコーチ。スクラム、カンバン、XPをサポート。

**主な機能**:
- スプリント計画とバックログ管理
- レトロスペクティブ（KPT法、5 Whys）
- ベロシティ計測と予測
- デイリースタンドアップ支援

**使用場面**: アジャイルチーム運営、プロセス改善

---

### 3. 🔌 **API Designer AI**
**ファイル**: `api-designer.md`

RESTful API、GraphQL、gRPCの設計を支援。OpenAPI/Swagger仕様書を自動生成。

**主な機能**:
- リソース設計とエンドポイント定義
- OpenAPI 3.0仕様書生成
- GraphQLスキーマ設計
- API認証・バージョニング戦略

**使用場面**: Web API設計、マイクロサービス開発

---

### 4. 🐛 **Bug Hunter AI**
**ファイル**: `bug-hunter.md`

バグの検出・分析・修正を支援する専門家。根本原因分析と再発防止策を提案。

**主な機能**:
- コード静的解析
- 根本原因分析（5 Whys、魚骨図）
- 修正コードの生成
- 再発防止策の提案

**使用場面**: バグ修正、コード品質向上

---

### 5. ☁️ **Cloud Architect AI**
**ファイル**: `cloud-architect.md`

AWS、Azure、GCPのクラウドアーキテクチャ設計。IaCコード（Terraform、Bicep）を生成。

**主な機能**:
- クラウドアーキテクチャ設計
- コスト最適化分析
- セキュリティ設計（ネットワーク、IAM）
- IaCコード生成（Terraform、Bicep）

**使用場面**: クラウド移行、インフラ設計

---

### 6. 👨‍💻 **Software Developer AI**
**ファイル**: `software-developer.md`

コード実装のスペシャリスト。複数言語・フレームワークで本番環境対応のコードを実装。

**主な機能**:
- REST API実装（TypeScript、Python、Go等）
- データベースアクセス層構築
- Azureサービス統合（Blob Storage、Key Vault）
- ユニットテスト・統合テスト生成

**使用場面**: コード実装、API構築、データベース連携

---

### 7. 🔍 **Code Reviewer AI**
**ファイル**: `code-reviewer.md`

コードレビューを自動化。可読性、パフォーマンス、セキュリティを網羅的にチェック。

**主な機能**:
- コード品質分析（命名規則、複雑度）
- セキュリティ脆弱性検出
- パフォーマンス改善提案
- ベストプラクティス適用

**使用場面**: プルリクエストレビュー、リファクタリング

---

### 8. 🗄️ **Database Schema Designer AI**
**ファイル**: `database-schema-designer.md`

データベース設計の専門家。ER図、正規化、インデックス戦略を提案。

**主な機能**:
- ER図作成（Mermaid形式）
- 正規化分析（1NF〜BCNF）
- インデックス設計
- DDL生成（PostgreSQL、MySQL）

**使用場面**: データベース設計、スキーマ移行

---

### 9. 🚀 **DevOps Engineer AI**
**ファイル**: `devops-engineer.md`

CI/CDパイプライン構築とインフラ自動化。Docker、Kubernetes、GitHub Actionsをサポート。

**主な機能**:
- CI/CD設定（GitHub Actions、GitLab CI）
- Dockerコンテナ化
- Kubernetes マニフェスト作成
- インフラ監視設定

**使用場面**: CI/CD構築、コンテナ化、自動デプロイ

---

### 10. 📊 **Observability Engineer AI**
**ファイル**: `observability-engineer.md`

システム可観測性の設計。Logs、Metrics、Tracesの3本柱を実装。

**主な機能**:
- 構造化ログ設計
- メトリクス収集（Prometheus）
- 分散トレーシング（OpenTelemetry）
- SLI/SLO/SLA定義

**使用場面**: 監視システム構築、障害対応

---

### 11. ⚡ **Performance Optimizer AI**
**ファイル**: `performance-optimizer.md`

パフォーマンスボトルネックの検出と最適化。アルゴリズム改善、キャッシング戦略を提案。

**主な機能**:
- ボトルネック分析
- N+1クエリ問題解決
- アルゴリズム最適化
- キャッシング戦略

**使用場面**: 速度改善、リソース最適化

---

### 12. 📋 **Project Manager AI**
**ファイル**: `project-manager.md`

プロジェクト計画、進捗管理、リスクマネジメントを支援。

**主な機能**:
- WBS作成
- ガントチャート生成
- リスク管理（リスクレジスター）
- ステークホルダー管理

**使用場面**: プロジェクト立ち上げ、進捗管理

---

### 13. ✅ **Quality Assurance AI**
**ファイル**: `quality-assurance.md`

品質保証戦略の策定。テスト計画、品質メトリクス測定。

**主な機能**:
- テスト戦略策定（テストピラミッド）
- 品質メトリクス定義
- テスト自動化計画
- 不具合管理

**使用場面**: QA戦略策定、品質改善

---

### 14. 📝 **Requirements Analyst AI**
**ファイル**: `requirements-analyst.md`

要件定義のスペシャリスト。ユーザーストーリー、機能要件、非機能要件を整理。

**主な機能**:
- ユーザーストーリー作成
- 機能要件・非機能要件定義
- MoSCoW優先順位付け
- SRS（ソフトウェア要求仕様書）生成

**使用場面**: プロジェクト初期、要件整理

---

### 15. 🔒 **Security Auditor AI**
**ファイル**: `security-auditor.md`

セキュリティ監査の専門家。OWASP Top 10準拠、脆弱性診断。

**主な機能**:
- OWASP Top 10チェック
- 脆弱性診断（SQLインジェクション、XSS）
- CVSS評価
- 修正コード提案

**使用場面**: セキュリティレビュー、脆弱性診断

---

### 16. 🏗️ **System Architect AI**
**ファイル**: `system-architect.md`

システムアーキテクチャ設計。C4モデル、ADR（Architecture Decision Records）を作成。

**主な機能**:
- C4モデル図作成
- ADR作成
- アーキテクチャパターン選定
- トレードオフ分析

**使用場面**: システム設計、技術選定

---

### 17. 📚 **Technical Writer AI**
**ファイル**: `technical-writer.md`

技術文書作成の専門家。API仕様書、README、開発者ガイドを生成。

**主な機能**:
- API仕様書作成
- README生成
- ユーザーマニュアル作成
- Mermaid図作成

**使用場面**: ドキュメント作成、API仕様書

---

### 18. 🧪 **Test Engineer AI**
**ファイル**: `test-engineer.md`

テスト設計・自動テスト生成。ユニット、統合、E2Eテストをカバー。

**主な機能**:
- テストケース設計（境界値分析、同値分割）
- ユニット/統合/E2Eテスト生成
- モック・スタブ設計
- カバレッジ分析

**使用場面**: テスト作成、カバレッジ向上

---

### 19. 🎨 **UI/UX Designer AI**
**ファイル**: `uiux-designer.md`

ユーザー中心設計。ワイヤーフレーム、デザインシステム、アクセシビリティ対応。

**主な機能**:
- ワイヤーフレーム作成
- デザインシステム構築
- アクセシビリティ（WCAG準拠）
- ユーザビリティテスト計画

**使用場面**: UI/UX設計、デザインシステム構築

---

## 🚀 使い方

### 1. エージェントの選択

プロジェクトのニーズに応じて、適切なエージェントを選択します。

**例**:
- API設計が必要 → **API Designer AI**
- データベース設計 → **Database Schema Designer AI**
- セキュリティチェック → **Security Auditor AI**
- 総合的なプロジェクト → **Orchestrator AI**（複数エージェントを自動選択）

### 2. プロンプトの使用

各エージェントプロンプトをAIアシスタント（GitHub Copilot、ChatGPT、Claude等）に読み込ませます。

```markdown
以下のプロンプトに従って、API設計を支援してください。

[api-designer.mdの内容をコピー＆ペースト]

---

私のリクエスト: ユーザー管理APIを設計したい
```

### 3. 対話フローに従う

各エージェントは**5つのフェーズ**で段階的に情報を収集します：

1. **フェーズ1: 初回ヒアリング** - 基本情報の収集（5-6問）
2. **フェーズ2: 詳細ヒアリング** - 専門的な要件の深堀り（5-7問）
3. **フェーズ3: 確認フェーズ** - 収集した情報の整理と確認
4. **フェーズ4: 成果物生成** - 設計書・コード・図の生成
5. **フェーズ5: フィードバック** - 修正・改善の反映

### 4. 成果物の受け取り

エージェントは以下のような成果物を生成します：

- **設計書**: Markdown形式（`.md`）
- **コード**: 実装可能なコードスニペット
- **図**: Mermaid形式の図
- **仕様書**: OpenAPI、ER図、テストケース等

---

## 📁 ファイル構造

```
.github/agents/
├── README.md                      # このファイル
├── orchestrator.md                # マルチエージェントオーケストレーター
├── agile-coach.md                # アジャイルコーチ
├── api-designer.md               # API設計
├── bug-hunter.md                 # バグ検出・修正
├── cloud-architect.md            # クラウドアーキテクチャ
├── code-reviewer.md              # コードレビュー
├── database-schema-designer.md   # データベース設計
├── devops-engineer.md            # DevOps/CI/CD
├── observability-engineer.md     # 可観測性設計
├── performance-optimizer.md      # パフォーマンス最適化
├── project-manager.md            # プロジェクト管理
├── quality-assurance.md          # 品質保証
├── requirements-analyst.md       # 要件分析
├── security-auditor.md           # セキュリティ監査
├── software-developer.md         # ソフトウェア開発（コード実装）
├── system-architect.md           # システムアーキテクチャ
├── technical-writer.md           # 技術文書作成
├── test-engineer.md              # テスト設計
└── uiux-designer.md              # UI/UX設計
```

---

## 🎯 エージェントの選び方

### プロジェクトフェーズ別

| フェーズ | 推奨エージェント |
|---------|----------------|
| **企画・要件定義** | Requirements Analyst, Project Manager |
| **設計** | System Architect, Database Schema Designer, API Designer |
| **実装** | Software Developer, Code Reviewer, Bug Hunter |
| **テスト** | Test Engineer, Quality Assurance |
| **デプロイ** | DevOps Engineer, Cloud Architect |
| **運用** | Observability Engineer, Performance Optimizer, Security Auditor |

### 課題別

| 課題 | 推奨エージェント |
|------|----------------|
| **APIを設計したい** | API Designer |
| **データベースを設計したい** | Database Schema Designer |
| **コードを実装したい** | Software Developer |
| **バグを修正したい** | Bug Hunter |
| **コードをレビューしてほしい** | Code Reviewer |
| **セキュリティをチェックしたい** | Security Auditor |
| **パフォーマンスを改善したい** | Performance Optimizer |
| **CI/CDを構築したい** | DevOps Engineer |
| **クラウドに移行したい** | Cloud Architect |
| **テストを自動化したい** | Test Engineer |
| **ドキュメントを作成したい** | Technical Writer |
| **UI/UXを改善したい** | UI/UX Designer |
| **プロジェクトを管理したい** | Project Manager |
| **アジャイル開発を導入したい** | Agile Coach |
| **複雑なプロジェクト全般** | Orchestrator（複数エージェントを自動選択） |

---

## 🌟 ベストプラクティス

### 1. **明確な目標を伝える**

エージェントに対して、達成したいことを明確に伝えましょう。

❌ **悪い例**: 「何か作って」
✅ **良い例**: 「RESTful APIでユーザー管理機能を設計したい。認証はJWT、データベースはPostgreSQLを使用」

### 2. **段階的に情報を提供する**

エージェントは1問1答形式で質問します。焦らず、1つずつ回答しましょう。

### 3. **既存情報を共有する**

既存のコード、仕様書、エラーメッセージがある場合は積極的に共有しましょう。

### 4. **フィードバックを提供する**

生成された成果物にフィードバックを提供することで、より精度の高い結果が得られます。

### 5. **複数エージェントを連携する**

複雑なプロジェクトでは、Orchestratorを使用して複数エージェントを連携させましょう。

**例**:
1. **Requirements Analyst** で要件定義
2. **System Architect** でアーキテクチャ設計
3. **API Designer** でAPI設計
4. **Database Schema Designer** でDB設計
5. **Test Engineer** でテスト設計
6. **DevOps Engineer** でCI/CD構築

---

## 📋 各エージェントの共通機能

全てのエージェントは以下の機能を標準装備しています：

### ✅ 対話フロー
- **1問1答形式**: 段階的に情報を収集
- **選択肢の提供**: a/b/c形式で回答しやすく
- **進捗の可視化**: 【質問3/5】のように進捗を表示

### ✅ ファイル出力
- **自動ファイル生成**: 設計書、仕様書、コードを自動生成
- **細分化ルール**: 大きな文書は複数ファイルに分割
- **ユーザー確認**: 各ファイル生成後に確認を求める

### ✅ ベストプラクティス
- **業界標準**: フレームワーク、手法、ツールを網羅
- **実装例**: すぐに使えるコードスニペット
- **禁止事項**: やってはいけないことを明示

### ✅ 品質保証
- **チェックリスト**: 成果物の品質を保証
- **レビュー**: 技術的正確性を検証
- **改善提案**: 継続的な改善をサポート

---

## 🔧 カスタマイズ

各エージェントプロンプトは、プロジェクトのニーズに応じてカスタマイズ可能です。

### カスタマイズ可能な項目

- **質問項目**: プロジェクト特有の質問を追加
- **選択肢**: 技術スタックに応じた選択肢に変更
- **出力形式**: 会社独自のテンプレートに変更
- **用語**: チーム内の用語に統一

### カスタマイズ例

```markdown
<!-- オリジナルの質問 -->
【質問2/5】使用するデータベースは？
a) PostgreSQL
b) MySQL
c) MongoDB

<!-- カスタマイズ後 -->
【質問2/5】使用するデータベースは？
a) PostgreSQL 15（推奨、当社標準）
b) MySQL 8.0
c) その他（理由を教えてください）
```

---

## 🤝 貢献

このプロジェクトへの貢献を歓迎します！

### 貢献方法

1. **Issue報告**: バグや改善提案をIssueで報告
2. **プルリクエスト**: 修正や新機能の追加
3. **フィードバック**: 使用感や改善案を共有

### 貢献ガイドライン

- **明確な説明**: 変更理由と期待される効果を記載
- **テスト**: 実際にAIで動作確認
- **フォーマット**: 既存のスタイルに従う
- **ドキュメント**: README.mdも適宜更新

---

## 📄 ライセンス

このプロジェクトは[MITライセンス](../../../LICENSE)の下で公開されています。

---

## 📞 サポート

### 質問・相談

- **GitHub Issues**: バグ報告、機能リクエスト
- **GitHub Discussions**: 使い方の質問、議論

### リソース

- [GitHub Copilot公式ドキュメント](https://docs.github.com/copilot)
- [プロンプトエンジニアリングガイド](https://platform.openai.com/docs/guides/prompt-engineering)

---

## 🎓 学習リソース

各エージェントで扱うトピックの学習リソース：

### アーキテクチャ・設計
- [C4 Model](https://c4model.com/)
- [Architecture Decision Records](https://adr.github.io/)
- [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)

### DevOps・インフラ
- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [Terraform Documentation](https://www.terraform.io/docs)
- [CNCF Cloud Native Trail Map](https://github.com/cncf/trailmap)

### セキュリティ
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [CWE Top 25](https://cwe.mitre.org/top25/)

### テスト
- [Test Pyramid](https://martinfowler.com/articles/practical-test-pyramid.html)
- [Testing Best Practices](https://github.com/goldbergyoni/javascript-testing-best-practices)

### UI/UX
- [Nielsen Norman Group](https://www.nngroup.com/)
- [WCAG 2.1 Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)

---

## 📊 統計情報

- **総エージェント数**: 19個
- **総行数**: 約20,000行
- **対応プログラミング言語**: Python, JavaScript/TypeScript, Java, Go, C#, SQL, YAML等
- **対応クラウド**: AWS, Azure, GCP
- **対応CI/CDツール**: GitHub Actions, GitLab CI, Jenkins, CircleCI

---

## 🎉 謝辞

このプロジェクトは、以下のフレームワーク・手法に基づいています：

- **デザインパターン**: Gang of Four, SOLID原則
- **アジャイル**: Scrum, Kanban, XP
- **アーキテクチャ**: C4 Model, ADR, Clean Architecture
- **セキュリティ**: OWASP, NIST, CIS Benchmarks
- **テスト**: Test Pyramid, BDD, TDD
- **DevOps**: DORA Metrics, SRE Practices

---

## 📝 更新履歴

### 2025-11-06
- Software Developer AI エージェントを追加（19個目）
- DevOps Engineer AI に Azure デプロイ実装例を追加（Azure Pipelines, GitHub Actions, Terraform）
- Orchestrator AI を17エージェントに更新

### 2025-01-15
- 初回リリース: 18個のエージェントプロンプトを公開
- 全エージェントに5フェーズ対話フロー実装
- ファイル出力の細分化ルール追加

---

**Spec Copilot - より良いAI体験を、すべての開発者に** 🚀
