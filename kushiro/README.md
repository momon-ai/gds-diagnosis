# 選ばれ続けるまち、釧路 — KUSHIRO BRANDING PROPOSAL

釧路市ブランドロゴ・キャッチコピーのデザイン公募向け提案書（応募用成果物）。

## 成果物
- **`釧路ブランド提案.pdf`** — 提出用の提案書（12スライド／16:9）
- `proposal.html` — 提案書のソース（フォント同梱・自己完結）
- `fonts/` — 埋め込みフォント（Noto Sans JP / Noto Serif JP / Space Grotesk, OFL）

## コンセプト
**課題:** 地方ブランドは「自然・食・人」に収束し、見分けがつかない。
**洞察:** 釧路は"これから選ばれたい"のではなく、**もう選ばれている**
（移住体験「ちょっと暮らし」全道1位・14年連続 ほか、真似できない実績）。
**核:** 「選ばれ続けるまち、釧路」— 市がめざす「選ばれるまち」を、14年の実績で裏づけて一段引き上げる。
**キャッチコピー（主案）:** 「また、来たくなる。ずっと、いたくなる。」
（観光＝再訪／長期滞在・二地域居住・移住＝定住 を一文で束ねる）
**ロゴ:** *The Meander & The Dot* — 蛇行する釧路川・湿原のリボン＋「選ばれた一点」＝丹頂の冠羽・世界三大夕日を表す赤いドット。

## 出典（数値・事実）
釧路市ホームページ「そもそもくしろってどんなまち？」／マーケティング戦略室 vol.1–3 ／ 楽待コラム（移住体験利用者数）。数値は令和6年度時点。

## PDFの再生成
```bash
# フォントを取得（npmレジストリ経由）
npm install
# HTML → PDF（Chromium ヘッドレス）
CHROME=/opt/pw-browsers/chromium-1194/chrome-linux/chrome  # 環境に合わせて変更
"$CHROME" --headless=new --no-sandbox --disable-gpu --allow-file-access-from-files \
  --no-pdf-header-footer --virtual-time-budget=8000 \
  --print-to-pdf=釧路ブランド提案.pdf "file://$PWD/proposal.html"
```
