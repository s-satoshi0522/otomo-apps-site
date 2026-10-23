# otomo-apps-site
オトモアプリのプライバシーポリシー・サポート情報を公開するサイト。

## 現在の状態

公開準備中です。テニスのオトモのプライバシーポリシーの施行日は2026年9月29日とします。オトモゲームズ Classicの施行日は公開前に確定します。公開URLの動作確認はまだ完了していません。

- [目次](index.html)
- [テニスのオトモのサポート](tennis-otomo/support.html)
- [テニスのオトモのプライバシーポリシー](tennis-otomo/privacy.html)
- [オトモゲームズ Classicのサポート](otomo-games-classic/support.html)
- [オトモゲームズ Classicのプライバシーポリシー](otomo-games-classic/privacy.html)

HTMLをブラウザで直接開いて確認できます。ビルド・外部ライブラリは不要です。
共通の問い合わせ先は `otomo.apps.support@gmail.com` です。
アプリごとに文書を分け、将来のアプリに同じ内容を自動適用しません。

## 更新と公開

1. featureブランチで変更し、本文と投稿予定のIssue・PR内容をチャットで人が確認する。投稿依頼を受けるまでGitHubへ投稿しない。
2. 本文の未確定事項、施行日、必要な表示、公開対象のファイル・全Git履歴・著者情報・Issue・PRに問題がないか確認する。
3. 相対リンク、HTML構造、スマートフォンとデスクトップでの表示、キーボード操作を確認する。
4. 未stageは `git diff --check`、stage済みは `git diff --cached --check`、commit済みは `git diff --check main...HEAD` で確認する。
5. 人の承認後にPRを投稿する。Mergeは人が行う。
6. 公開の明示承認後、施行日と本文の公開準備用の表記を確認する。公開が予定日から遅れた場合は、施行日の扱いを人に確認する。`noindex` は検索制御であってアクセス制限ではないため、準備中はPages自体を有効化しない。
7. 人の承認に従いリポジトリをPublicにし、GitHub Pagesの公開元を `main` のルートに設定する。公開前に未確定事項がないことを再確認する。
8. ログインしていないブラウザでHTTPSアクセス、文書・CSS・履歴リンク・問い合わせ先を確認する。実際の公開URLと確認日を記録する。

想定パスは、プライバシーポリシーが `/otomo-apps-site/tennis-otomo/privacy.html`、サポートが `/otomo-apps-site/tennis-otomo/support.html` です。公開確認前にApp Storeへ提出しないでください。
アプリ本体のリポジトリの公開設定は、このサイトの公開とは別です。

## 参考資料

- [Firebaseのプライバシーとセキュリティ](https://firebase.google.com/support/privacy)
- [AppleのApp Reviewガイドライン](https://developer.apple.com/app-store/review/guidelines/#privacy)
- [ヘルスケアデータの管理](https://support.apple.com/ja-jp/108779)
- [GitHub Pagesについて](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)

## オトモゲームズ Classicの掲載内容

想定パスは、サポートが `/otomo-apps-site/otomo-games-classic/support.html`、プライバシーポリシーが `/otomo-apps-site/otomo-games-classic/privacy.html` です。

2026年10月23日に、Classicのcommit `de794869f6b4f9ceaebf839d1b2cf76dbfcc7c02` のゲーム起動・保存処理、iOS / Androidの依存関係と設定を確認して記載しています。ゲームの一時状態と動画の視聴済み・解放状態を区別し、iOS版固有の保存情報をAndroid版へ自動適用しません。問い合わせ窓口の保存・削除方針は既存サイトの運用に合わせています。

2026年10月24日に、Classicのcommit `91e29d385f8cadd69e2384357c297567a45cb518` と `docs/setup/245_classic_crashlytics.md` を確認し、iOS / Android配布版のFirebase Crashlyticsによる自動収集を反映しました。テニスのオトモと同じ方針で、利用目的、送信内容、収集切替設定の有無、保持・削除の説明を記載しています。

公開前には、配布対象のClassicの実装・利用サービスとの再照合、施行日の確定と準備中表記の更新、対応環境・公開URLの確認を行ってください。ストアURLは掲載していません。
