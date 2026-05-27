# 手値（Tene）詳細検索インデックス
> 「あのときどうやったっけ」を調べるときに使う

## PWA関連
- **manifest.jsonの場所**: リポジトリルート（icons/サブフォルダではない）
- **アイコン生成**: generate-icons.htmlをGitHub Pagesで開いてダウンロード
- **フィーチャーグラフィック生成**: generate-feature.htmlで生成（1024x500px）

## PWABuilder関連
- **URL**: https://www.pwabuilder.com/
- **Package IDの注意**: `io.github.keronimo119_ui.twa`ではなく`io.github.keronimo119ui.tene`
- **署名キーエラー**: 毎回新しいキーを使うと署名不一致エラーになる→必ずVr1のsigning.keystoreを使う
- **バージョンコードエラー**: 同じバージョンコードは使えない→毎回+1する

## Play Console関連
- **コンテンツのレーティング**: IARCアンケート送信が必要、保存だけではダメ
- **広告IDエラー**: 「申告を完了する」→「いいえ」で解決
- **AAB署名不一致エラー**: PWABuilderでUse mine→Vr1のsigning.keystoreを使う
- **バージョンコード重複エラー**: PWABuilderでVersion codeを前回+1にする
- **タブレットスクリーンショット**: 必須ではない、スマホ2枚でOK

## ストア掲載情報
- **アプリ名**: 手値 - Tene
- **カテゴリ**: 仕事効率化
- **プライバシーポリシーURL**: https://keronimo119-ui.github.io/tene/privacy-policy.html
- **連絡先メール**: keronimo119@gmail.com

## クローズドテスト
- **テスター数**: 12人必要（オプトインクリックのみでOK、実際の使用不要）
- **期間**: 14日間
- **メーリングリスト名**: Teneテスター
