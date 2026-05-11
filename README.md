# Watch / Clock Breakdown Worksheet Generator

時計を国際発送する際にアメリカ通関で要求される **Watch / Clock Breakdown Worksheet** をブラウザだけで作成できる Web ツール。

## 使い方

公開URL を開く → 注文情報を入力 → 「📄 PDFを作成してダウンロード」ボタン

完全にブラウザ内で動作するため、注文データはサーバーに送信されません。

## 対応キャリア

DHL / FedEx / UPS いずれの追跡番号でも利用可。フォームは特定キャリア専用ではなく、US Customs (19 CFR 141.86) の要求事項に沿った汎用フォーマット。

## 自動判定

eBay の商品タイトルを貼り付けると以下を自動推定:

- ムーブメント種類 (Analogue / Digital)
- 電源タイプ (Battery / Wind Up / Self-Winding)
- ストラップ素材
- ケース素材
- 宝石数
- 電池型番 (SR626SW / CR2016 等)

判定結果は手動で上書き可能。

## 金額按分

販売額 (USD) を入力すると、Movement / Case / Strap / Battery に自動分配:

| 電源 | Movement | Case | Strap | Battery |
|------|----------|------|-------|---------|
| Battery (Quartz) | 80% | 10% | 7% | 3% |
| Self-Winding / Wind Up | 80% | 10% | 10% | 0% |

端数は Movement に寄せて、合計が必ず販売額に一致するよう調整。

## 注意

- ワニ革・象牙等の CITES 対象素材は別途書類が必要（本ツール対象外）
- 金額は USD 固定
