# Instagram 数値チェック キット

他社・公開アカウントの **フォロワー数や投稿への反応（いいね数・コメント数）を、スマホで日々眺める** ための一式です。
AIアシスタント「Muse」を使う前提で、**特別な開発・API申請は不要**です。

---

## 本橋さんへ：進め方はこれだけです

### 手順 1 ― まず Muse に登録する
📄 [01_muse_getting_started.pdf](01_muse_getting_started.pdf) を開いて、その通りに登録してください。
**初日は登録が終わればOKです。**

### 手順 2 ― 登録できたら、Muse のチャットにこのリポジトリの URL を貼って、こう送る
```text
このリポジトリを読んで、設定方法を教えてください。
https://github.com/kentsoda/instagram-check-kit
```
あとは Muse が順番に案内します。初回は「Instagramの連携」と「見たいアカウントを伝える」ところまでで終わります。

### 手順 3 ― 見た目の好みを伝える
🎨 [03_numbers_template.html](https://kentsoda.github.io/instagram-check-kit/03_numbers_template.html) を開くと、数値ページのデザインが **3パターン（A：カード型／B：一覧表型／C：グラフ型）** 切り替えて見られます。
気に入った記号を Muse に伝えるだけです（後から変更もできます）。

---

## ファイル一覧

| ファイル | 内容 | いつ見る |
|---|---|---|
| [01_muse_getting_started.pdf](01_muse_getting_started.pdf) | **資料1**：Museの簡単な説明と登録方法 | 最初に1回 |
| [02_instagram_guide.html](https://kentsoda.github.io/instagram-check-kit/02_instagram_guide.html) ／ [PDF版](02_instagram_guide.pdf) | **資料2**：数値チェックのはじめ方ガイド（スマホ用） | 登録後、設定しながら |
| [03_numbers_template.html](https://kentsoda.github.io/instagram-check-kit/03_numbers_template.html) | **資料3**：実際の数値ページのテンプレート（デザイン3パターン切替・数値はサンプル） | 見た目を選ぶとき |
| [04_spec_for_muse.md](04_spec_for_muse.md) | **資料4**：Muse に読ませる仕様書 兼 指示書 v2 | Muse が読むもの（人は読まなくてOK） |
| この README | 入口と、Muse への指示 | ― |

スマホで読む用の Web 版（GitHub Pages）：
- ガイド： https://kentsoda.github.io/instagram-check-kit/02_instagram_guide.html
- テンプレート： https://kentsoda.github.io/instagram-check-kit/03_numbers_template.html

---

## Muse へ（このリポジトリを読んだ AI への指示）

利用者がこのリポジトリの URL を貼って「設定方法を教えて」等と依頼したら、次を実行してください。

1. **まず [04_spec_for_muse.md](04_spec_for_muse.md) を全文読む**。以降の案内はその仕様に従う。
2. 利用者はスマホのみで使う前提。案内は短文・箇条書き・番号付き選択肢で、一度に1ステップだけ進める。
3. 初回は仕様 §3 の範囲（Instagram連携の確認 → 対象アカウントの一覧提示と確認）で止める。取得項目の細部は初回に決めさせない。
4. デザインは資料3の A／B／C、見せ方は仕様 §5 の ①HTMLファイル ②共有URL ③Museスペース から選んでもらう（後日でも可）。
5. 取れない数値（再生数・保存数・フォロワー属性など）を推測で埋めない。認証情報をチャットで受け取らない。
6. 利用者がファイルを個別に渡してきた場合も、扱いは同じ（04 が正）。

---

## できること・できないこと（要点）

- ✅ 公開アカウントのフォロワー数・投稿数、投稿ごとのいいね数・コメント数、日々の増減
- ❌ 再生数・保存数・シェア数、フォロワー属性（年齢・性別・地域）― 所有者本人しか見られず、公式APIでも第三者には公開されていません
- 📌 過去の推移はさかのぼれません。今日から貯めた分だけが並びます

---

*作成：2026-11-24 / 仕様 v2.0*
