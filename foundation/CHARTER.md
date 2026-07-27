# Humaicraft Charter

This charter defines the purpose, authority, and operating boundaries of Humaicraft.

## 1. Purpose

Humaicraft exists to help people and AI build software that is safe, understandable, maintainable, accessible, reproducible, and able to grow over time.

It does this through shared philosophy, practical guidelines, reusable tools, working products, documented decisions, and open learning.

## 2. Scope

Humaicraft may include:

- foundation documents and shared principles;
- engineering, security, accessibility, documentation, and operational guidelines;
- reference architectures, patterns, templates, and playbooks;
- software products that demonstrate the philosophy in practice;
- decision records, lessons, and community knowledge.

Each product may define project-specific rules, but those rules should not silently weaken the Foundation.

## 3. Human Authority

Humans retain final judgment, responsibility, and authority.

AI may assist with research, planning, implementation, testing, review, documentation, and maintenance. AI must not independently finalize consequential decisions, destructive operations, releases, permission changes, or public claims without the required human approval.

## 4. Decision Priority

When priorities conflict, decisions should follow this order:

1. safety of users and data;
2. correctness and reliability;
3. understandability and maintainability;
4. accessibility;
5. reproducibility and operability;
6. performance;
7. development speed;
8. implementation convenience.

A project may add stricter requirements, but should document any exceptional departure from this order.

## 5. Working Method

Humaicraft favors a focused, iterative cycle:

1. clarify purpose, users, requirements, constraints, risks, tests, and completion conditions;
2. build the smallest responsible change;
3. review purpose, design, security, accessibility, tests, operations, and documentation;
4. fix release-blocking findings;
5. record future improvements as issues or roadmap items;
6. release with migration and rollback information when relevant;
7. reflect on what was built and learned.

New ideas should be preserved without disrupting the current milestone.

## 6. Quality and Evidence

Work must not be presented as verified unless it has actually been verified.

Projects should provide tests or reproducible validation appropriate to their risk. Failures, partial success, missing configuration, and known limitations must be reported honestly.

Security-sensitive information must not be committed to code, documentation, logs, fixtures, or generated artifacts.

## 7. Accessibility

Humaicraft treats accessibility as part of quality.

Projects should aim for WCAG 2.2 AA unless stronger requirements apply, and should consider semantic structure, keyboard operation, focus behavior, understandable errors, reduced motion, and non-visual use from the beginning.

## 8. Documentation and Decisions

Important decisions that cannot be understood from the result alone must be recorded.

Depending on significance, projects should use ADRs, decision logs, issues, pull requests, design documents, changelogs, roadmaps, or lessons.

Documentation should be updated with the change it describes.

## 9. Failure and Learning

Humaicraft does not celebrate carelessness and does not hide honest failure.

When something goes wrong, projects should examine what happened, its impact, contributing conditions, corrective action, and how recurrence will be prevented. Useful lessons should be preserved and shared without turning reflection into blame.

## 10. Governance

Foundation changes require deliberate review because they affect the whole ecosystem.

A proposed change should explain:

- the problem or opportunity;
- why the Foundation should change;
- affected documents and projects;
- risks and trade-offs;
- migration or adoption considerations;
- how the change will be reviewed.

Project maintainers may make local decisions within their scope. Decisions that conflict with the Foundation must be made explicit and reviewed rather than introduced silently.

## 11. Evolution

Humaicraft is a living project.

Releases are milestones, not finish lines. The Foundation may evolve when practice reveals better understanding, but changes should preserve continuity, explain their reasons, and avoid unnecessary disruption.

---

# Humaicraft 憲章

この憲章は、Humaicraftの目的、権限、活動上の境界を定めます。

## 1. 目的

Humaicraftは、人とAIが、安全で、理解しやすく、保守可能で、アクセシブルで、再現でき、長く育てられるソフトウェアをつくれるようにするために存在します。

共通の思想、実践的なガイドライン、再利用可能なツール、実際に動くプロダクト、判断記録、オープンな学びを通じて、その目的を実現します。

## 2. 対象範囲

Humaicraftには、次のものを含めることができます。

- Foundation文書と共通原則
- 開発、セキュリティ、アクセシビリティ、ドキュメント、運用のガイドライン
- 参照アーキテクチャ、パターン、テンプレート、プレイブック
- 思想を現実の利用で示すソフトウェアプロダクト
- 判断記録、失敗からの学び、コミュニティの知識

各プロダクトは固有のルールを定められますが、Foundationを暗黙的に弱めてはいけません。

## 3. 人間の権限

最終的な判断、責任、権限を持つのは人間です。

AIは、調査、計画、実装、テスト、レビュー、ドキュメント、保守を支援できます。重大な判断、破壊的操作、リリース、権限変更、対外的な主張を、必要な人間の承認なしに確定してはいけません。

## 4. 判断の優先順位

優先事項が衝突した場合は、次の順で判断します。

1. 利用者とデータの安全
2. 正しさと信頼性
3. 理解しやすさと保守性
4. アクセシビリティ
5. 再現性と運用性
6. パフォーマンス
7. 開発速度
8. 実装上の便利さ

各プロジェクトは、より厳しい要件を追加できます。この順序から例外的に外れる場合は、その理由を記録します。

## 5. 作業方法

Humaicraftは、集中した反復サイクルを基本とします。

1. 目的、利用者、要件、制約、リスク、テスト、完了条件を整理する
2. 責任を持てる最小の変更をつくる
3. 目的、設計、セキュリティ、アクセシビリティ、テスト、運用、ドキュメントをレビューする
4. リリース前に必要な指摘を修正する
5. 将来の改善をIssueまたはロードマップへ残す
6. 必要に応じて移行・ロールバック情報とともにリリースする
7. 作ったものと学んだことを振り返る

新しいアイデアは、現在のマイルストーンを妨げずに記録します。

## 6. 品質と根拠

実際に検証していない作業を、検証済みとして表現してはいけません。

プロジェクトは、リスクに応じたテストまたは再現可能な検証を用意します。失敗、部分的成功、設定不足、既知の制約を正直に報告します。

秘密情報を、コード、ドキュメント、ログ、テストデータ、生成物へ記録してはいけません。

## 7. アクセシビリティ

Humaicraftは、アクセシビリティを品質の一部として扱います。

より強い要件がない限りWCAG 2.2 AAを意識し、セマンティックな構造、キーボード操作、フォーカス、理解できるエラー、動きの低減、視覚に依存しない利用を最初から考慮します。

## 8. ドキュメントと判断

成果物だけでは理解できない重要な判断は記録します。

重要度に応じて、ADR、決定ログ、Issue、Pull Request、設計文書、CHANGELOG、ROADMAP、Lessonsを使います。

ドキュメントは、対象となる変更と同時に更新します。

## 9. 失敗と学び

Humaicraftは雑さを称賛せず、正直な失敗を隠しません。

問題が起きた時は、何が起きたか、影響、背景条件、是正内容、再発防止策を確認します。振り返りを個人への非難にせず、有益な学びを残し、共有します。

## 10. ガバナンス

Foundationの変更はエコシステム全体へ影響するため、慎重にレビューします。

変更提案には、次を含めます。

- 解決する問題または機会
- Foundationを変更する理由
- 影響を受ける文書とプロジェクト
- リスクとトレードオフ
- 移行または採用時の考慮
- レビュー方法

各プロジェクトのメンテナーは、担当範囲内で判断できます。Foundationと衝突する判断は、暗黙的に導入せず、明示してレビューします。

## 11. 進化

Humaicraftは、生き続けるプロジェクトです。

リリースはゴールではなく節目です。実践からより良い理解が得られた時、Foundationは進化できます。ただし、継続性を守り、変更理由を説明し、不必要な混乱を避けます。
