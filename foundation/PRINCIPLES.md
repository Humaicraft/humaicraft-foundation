# Principles

Humaicraft's principles turn our values into practical decision-making guidance.

They do not replace professional judgment or project-specific requirements. They help people and AI make choices consistently, explain why those choices were made, and recognize when a decision should be reviewed.

Each principle includes its intent and examples of how it should influence real work.

## 1. People Before Technology

Technology should serve people, not require people to serve the technology.

### Why

Software affects users, operators, maintainers, contributors, and communities. Technical elegance has little value when it creates avoidable harm, exclusion, confusion, or operational burden.

### In practice

- Keep human responsibility and final authority explicit.
- Design for real abilities, environments, constraints, and failure modes.
- Prefer understandable workflows over impressive but opaque automation.
- Do not use AI or automation to hide accountability.

## 2. Safety Before Speed

When safety and delivery speed conflict, protect people and data first.

### Why

A fast release can be reversed. Harm to users, exposed data, lost trust, and destructive operations may not be reversible.

### In practice

- Use safe defaults and require deliberate confirmation for destructive actions.
- Validate external input and verify authorization for each protected operation.
- Stop safely when critical information is missing or uncertain.
- Do not report partial or unverified work as successful.

## 3. Correctness Before Convenience

Prefer behavior that is correct and trustworthy over behavior that is merely easy to implement.

### Why

Convenient shortcuts often move complexity into production, operations, or future maintenance. Correctness creates a stable base for later improvement.

### In practice

- Make requirements and assumptions explicit.
- Handle errors rather than hiding them.
- Test normal paths, failure paths, boundaries, permissions, and missing configuration.
- Do not weaken requirements only to make tests pass or deadlines easier.

## 4. Design with Intent

Every meaningful structure and dependency should have a clear reason to exist.

### Why

Accidental design is difficult to explain, maintain, and change. Intentional design makes responsibilities, constraints, and extension points visible.

### In practice

- Separate presentation, domain logic, data access, external integrations, and configuration.
- Keep functions, modules, and changes focused on one clear responsibility.
- Introduce abstraction where replacement or variation is reasonably expected.
- Avoid abstraction that has no present purpose or credible future need.

## 5. Make the Important Explicit

Important behavior, risk, configuration, and reasoning should be visible rather than implied.

### Why

Implicit systems depend on memory and hidden knowledge. Explicit systems are easier to review, operate, transfer, and trust.

### In practice

- Prefer named configuration and documented decisions over magic values and hidden behavior.
- Record significant trade-offs in ADRs, issues, pull requests, or design documents.
- Make permissions, environments, side effects, and destructive consequences clear.
- Use names that reveal responsibility and intent.

## 6. Build for the People Who Come Next

Create work that can be understood, maintained, and extended by people who were not present when it was made.

### Why

Software usually outlives its original context. Future maintainers should not need to reconstruct essential knowledge through guesswork.

### In practice

- Preserve the reason behind non-obvious decisions.
- Keep changes focused and avoid unrelated refactoring.
- Update documentation, tests, roadmap, and change history with the implementation.
- Provide migration and rollback paths for risky or breaking changes.

## 7. Accessibility Is Part of Quality

Accessibility is a core quality requirement, not an optional enhancement.

### Why

A product cannot be considered high quality when people are unnecessarily prevented from using it.

### In practice

- Aim for WCAG 2.2 AA unless stronger project requirements apply.
- Prefer semantic HTML and native controls.
- Support keyboard operation, visible focus, understandable errors, and reduced motion.
- Do not communicate meaning by color alone.

## 8. Build Small, Validate, and Grow

Create the smallest responsible step, verify it, and use what is learned to guide the next step.

### Why

Small changes are easier to understand, review, test, release, and reverse. They reduce risk without requiring careless shortcuts.

### In practice

- Keep one issue, pull request, and commit focused on a clear purpose where practical.
- Release in reviewable increments rather than waiting for imaginary perfection.
- Define completion before implementation begins.
- Record useful ideas without allowing them to disrupt the current milestone.

## 9. Review Is a Place to Grow

Review exists to improve the work and preserve trust, not to rank or diminish people.

### Why

Good review reveals risks, strengthens shared understanding, and creates better decisions. A blame-oriented culture hides uncertainty and mistakes.

### In practice

- Critique ideas and outcomes without attacking people.
- Review purpose, design, security, accessibility, tests, operations, and documentation.
- Distinguish release-blocking changes from future improvements.
- Convert useful findings into clear issues rather than losing them in conversation.

## 10. Preserve the Why

Record the reasoning, constraints, alternatives, and lessons behind meaningful decisions.

### Why

Code and final documents show what exists, but often cannot explain why it exists. Preserved reasoning prevents repeated mistakes and enables responsible change.

### In practice

- Use ADRs for significant architectural decisions and lighter decision logs for smaller choices.
- Explain constraints and trade-offs in pull requests.
- Document why a surprising implementation is necessary.
- Keep sensitive information out of documentation and logs.

## 11. Learn from Failure Without Normalizing Carelessness

Do not hide failure. Examine it, preserve what it teaches, and improve the system.

### Why

Failure can reveal weak assumptions, missing safeguards, and unclear processes. Learning is lost when failure is concealed, blamed on individuals, or repeated without reflection.

### In practice

- Separate honest learning from avoidable negligence.
- Record what happened, contributing conditions, impact, and corrective action.
- Add regression tests or reproducible checks when possible.
- Improve the process, documentation, or safeguards that allowed the problem to recur.

## 12. AI Is a Teammate, Not a Replacement

Use AI to strengthen human craftsmanship while keeping judgment, responsibility, and accountability with people.

### Why

AI can explore, draft, compare, review, and preserve context, but it can also produce confident errors and obscure assumptions.

### In practice

- Verify AI-generated outputs before relying on them.
- Do not claim that unperformed tests, reviews, or checks were completed.
- Make uncertainty and important assumptions visible.
- Keep human approval for consequential decisions and destructive operations.

## 13. Improve Before Expanding

Strengthen existing foundations before adding unnecessary scope or complexity.

### Why

Uncontrolled expansion creates fragile systems, unfinished work, and hidden operational costs. Durable growth depends on finishing, reviewing, and learning from what already exists.

### In practice

- Protect the current milestone from unrelated additions.
- Record new ideas as issues or roadmap candidates.
- Address significant safety, correctness, and maintainability gaps before expanding.
- Prefer a completed, reviewable step over many partially started steps.

## 14. Leave It Better

Do not leave the project in a worse state than you found it.

### Why

Small acts of care compound over time. Small acts of neglect do too.

### In practice

- Remove temporary code, obsolete comments, unused files, and accidental secrets.
- Improve nearby clarity when it is directly related and low risk.
- Avoid mixing broad cleanup into an unrelated change.
- Leave a clear next step when work cannot be completed safely.

## 15. Enjoy the Craft

Take responsibility seriously while preserving curiosity, satisfaction, and room to learn.

### Why

Healthy teams need more than productivity. Sustainable craftsmanship depends on trust, curiosity, shared progress, and the ability to experiment safely.

### In practice

- Celebrate meaningful progress, not only large releases.
- Create room for questions and respectful disagreement.
- Share useful discoveries and lessons.
- Avoid processes that add burden without improving safety, clarity, or quality.

---

# 原則

Humaicraftの原則は、価値観を現実の判断へつなげるための指針です。

専門家としての判断や、各プロジェクト固有の要件を置き換えるものではありません。人とAIが一貫した基準で選択し、その理由を説明し、見直すべき判断に気づけるようにするものです。

各原則では、その意図と、実際の仕事へどのように反映するかを示します。

## 1. 技術より人を優先する

技術は人を支えるために使い、人が技術へ従う状態をつくらない。

### 理由

ソフトウェアは、利用者、運用者、保守担当者、コントリビューター、コミュニティへ影響します。回避できる被害、排除、混乱、運用負担を生むなら、技術的な美しさだけでは価値になりません。

### 実践

- 人間の責任と最終判断を明示する。
- 実際の能力、環境、制約、失敗時の状況を考慮して設計する。
- 見栄えは良くても不透明な自動化より、理解可能な手順を選ぶ。
- AIや自動化によって責任の所在を曖昧にしない。

## 2. 速度より安全を優先する

安全性と開発速度が衝突する場合は、利用者とデータを守る。

### 理由

早いリリースは戻せる場合があります。しかし、利用者への被害、データ漏えい、失われた信頼、破壊的な操作は元に戻せないことがあります。

### 実践

- 安全側の初期値を使い、破壊的操作には意図的な確認を求める。
- 外部入力を検証し、保護対象ごとに認可を確認する。
- 重要な情報が不足または不確かな場合は、安全側に停止する。
- 部分的または未検証の作業を成功として報告しない。

## 3. 便利さより正しさを優先する

実装が簡単であることより、正しく信頼できる挙動を選ぶ。

### 理由

便利な近道は、複雑さを本番環境、運用、将来の保守へ移すことがあります。正しさは、その後の改善を支える安定した土台になります。

### 実践

- 要件と前提を明示する。
- エラーを隠さず、適切に処理する。
- 正常系、異常系、境界値、権限不足、設定不足を確認する。
- テストを通すことや納期を楽にするために、本来の要件を弱めない。

## 4. 意図を持って設計する

意味のある構造と依存関係には、存在する理由を持たせる。

### 理由

偶然できた設計は、説明、保守、変更が難しくなります。意図のある設計は、責務、制約、拡張点を見える状態にします。

### 実践

- 表示、ドメインロジック、データアクセス、外部連携、設定を分離する。
- 関数、モジュール、変更を一つの明確な責務へ集中させる。
- 差し替えや変化が現実的に予想される箇所には抽象化を検討する。
- 現在の目的も信頼できる将来要件もない抽象化は避ける。

## 5. 重要なことを明示する

重要な挙動、リスク、設定、判断理由を暗黙の状態にしない。

### 理由

暗黙的なシステムは、記憶や属人的な知識へ依存します。明示的なシステムは、レビュー、運用、引き継ぎ、信頼を支えます。

### 実践

- マジックナンバーや隠れた挙動より、名前の付いた設定と記録された判断を使う。
- 重要なトレードオフをADR、Issue、Pull Request、設計文書へ残す。
- 権限、環境、副作用、破壊的操作の影響を明確にする。
- 名前から責務と意図が分かるようにする。

## 6. 次に受け取る人のためにつくる

当時を知らない人でも理解し、保守し、拡張できる仕事を残す。

### 理由

ソフトウェアは、最初に存在した文脈より長く残ることがあります。将来の保守担当者に、推測だけで重要な知識を復元させるべきではありません。

### 実践

- 自明でない判断の理由を残す。
- 変更を必要な範囲へ集中させ、無関係なリファクタリングを混ぜない。
- 実装とともにドキュメント、テスト、ロードマップ、変更履歴を更新する。
- リスクのある変更や破壊的変更には、移行とロールバックの手順を用意する。

## 7. アクセシビリティを品質として扱う

アクセシビリティを追加機能ではなく、品質の基本要件として扱う。

### 理由

不必要な障壁によって人が利用できないプロダクトは、高品質とは言えません。

### 実践

- より強い要件がない限り、WCAG 2.2 AAを意識する。
- セマンティックHTMLとネイティブな操作要素を優先する。
- キーボード操作、視認できるフォーカス、理解できるエラー、動きの低減設定に対応する。
- 色だけで意味を伝えない。

## 8. 小さくつくり、検証し、育てる

責任を持てる最小単位でつくり、検証し、学びを次の一歩へ反映する。

### 理由

小さな変更は理解、レビュー、テスト、公開、取り消しが容易です。雑な近道を使わずにリスクを下げられます。

### 実践

- 可能な限り、一つのIssue、Pull Request、コミットを明確な一目的へ集中させる。
- 存在しない完璧を待たず、レビュー可能な単位で公開する。
- 実装前に完了条件を定義する。
- 有益なアイデアは記録し、現在のマイルストーンを妨げないようにする。

## 9. レビューを成長の場にする

レビューは、人を評価したり否定したりするためではなく、仕事と信頼を育てるために行う。

### 理由

良いレビューは、リスクを発見し、共通理解を深め、判断を改善します。非難を中心とした文化では、不確実さや失敗が隠されます。

### 実践

- 人を攻撃せず、考えと成果について議論する。
- 目的、設計、セキュリティ、アクセシビリティ、テスト、運用、ドキュメントを確認する。
- リリース前に必要な修正と、将来の改善を分ける。
- 有益な指摘を会話の中で失わず、明確なIssueへ変える。

## 10. 判断理由を残す

重要な判断の背景にある理由、制約、代替案、学びを記録する。

### 理由

コードや完成した文書から、存在するものは分かっても、なぜ存在するかまでは分からないことがあります。判断理由は、同じ失敗を防ぎ、責任ある変更を可能にします。

### 実践

- 重要なアーキテクチャ判断にはADRを使い、小さな判断には軽量な決定記録を使う。
- Pull Requestへ制約とトレードオフを書く。
- 意外に見える実装が必要な理由を説明する。
- ドキュメントとログへ秘密情報を残さない。

## 11. 雑さを正当化せず、失敗から学ぶ

失敗を隠さず、振り返り、得られた学びを残し、仕組みを改善する。

### 理由

失敗は、弱い前提、不足した安全策、不明確な手順を明らかにします。失敗を隠す、個人だけを責める、振り返らず繰り返すことで、学びは失われます。

### 実践

- 正直な学びと、避けられた不注意を区別する。
- 起きたこと、背景条件、影響、是正内容を記録する。
- 可能な限り、再発防止テストまたは再現可能な検証を追加する。
- 再発を許したプロセス、文書、安全策を改善する。

## 12. AIを代替ではなくチームメイトとして扱う

AIによって人間のクラフトマンシップを強くし、判断、責任、説明責任は人間が持つ。

### 理由

AIは、探索、草案作成、比較、レビュー、文脈の保存を支援できます。一方で、確信を持った誤りを生成したり、前提を見えにくくしたりすることもあります。

### 実践

- AIが生成した成果を、利用前に検証する。
- 実行していないテスト、レビュー、確認を完了済みと表現しない。
- 不確実さと重要な前提を明示する。
- 重大な判断や破壊的操作には、人間の承認を残す。

## 13. 拡張する前に改善する

スコープや複雑さを増やす前に、現在の土台を強くする。

### 理由

制御されない拡張は、壊れやすいシステム、未完成の仕事、見えない運用コストを生みます。長く続く成長には、今あるものを完成させ、レビューし、学ぶことが必要です。

### 実践

- 現在のマイルストーンを無関係な追加から守る。
- 新しいアイデアはIssueまたはロードマップ候補として記録する。
- 拡張前に、安全性、正しさ、保守性の重大な不足へ対応する。
- 多くの未完成な作業より、完成しレビュー可能な一歩を優先する。

## 14. 受け取った時より良い状態で残す

プロジェクトを、受け取った時より悪い状態で残さない。

### 理由

小さな配慮は時間とともに積み重なります。小さな放置も同じです。

### 実践

- 一時的なコード、古いコメント、未使用ファイル、誤って含まれた秘密情報を残さない。
- 変更と直接関係し、低リスクである場合は、周辺の分かりやすさも改善する。
- 無関係な大規模整理を同じ変更へ混ぜない。
- 安全に完了できない場合は、明確な次の作業を残す。

## 15. つくることを楽しむ

責任には真剣に向き合いながら、好奇心、達成感、学ぶ余白を守る。

### 理由

健全なチームには、生産性以外のものも必要です。持続可能なクラフトマンシップは、信頼、好奇心、共有された前進、安全に試せる環境によって支えられます。

### 実践

- 大きなリリースだけでなく、意味のある前進を祝う。
- 質問や敬意ある異論を歓迎する。
- 役立つ発見と学びを共有する。
- 安全性、明確さ、品質を高めない負担だけのプロセスを避ける。
