# 手値（Tene）実施プロセス
> 成功した手順のみ記録。失敗・試行錯誤はカット済み。

## Phase 1: バグ修正（完了）
1. iichi販売プラットフォームボタン追加
2. 売上一覧の月別フィルタ追加
3. 作品追加/編集でヘッダー表示切替
4. 価格計算ページの手数料修正
5. init()をtry-catch-finallyでラップ
6. 制作ログの「編集中作品のログ」ラベル削除
7. イベント日付の曜日表示修正

## Phase 2: PWA化（完了）
1. manifest.jsonをリポジトリルートに作成
2. sw.jsをリポジトリルートに作成
3. アイコン（icon-192.png / icon-512.png）はルートに配置済み
4. generate-icons.htmlでアイコン生成

## Phase 3: Google Play出品（進行中）

### Play Console設定
1. Googleアカウントでデベロッパー登録（25ドル）
2. アプリ名: 手値 - Tene
3. パッケージID: io.github.keronimo119ui.tene
4. カテゴリ: 仕事効率化

### AAB生成手順（PWABuilder）
1. https://www.pwabuilder.com/ でURLを入力
2. Package ID: `io.github.keronimo119ui.tene`（TWAではなくteneにすること）
3. Version code: 新しいリリースは前回+1にする
4. Signing key: Use mine → Vr1フォルダのsigning.keystoreを使用
5. Key alias: tene-key / Password: （signing-key-info.txtを参照）

### クローズドテスト設定
1. テスター12人のGmailをメーリングリストに登録
2. AABをアップロード（バージョンコードは毎回+1）
3. 審査送信 → 通過後オプトインリンクを12人に送る
4. 14日間テスト後に製品版申請

## Phase 4: AdMob（未着手）
- AdMobアカウント作成
- バナー広告ユニットID取得
- tene.htmlに広告コード追加
