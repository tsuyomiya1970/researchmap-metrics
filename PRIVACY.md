# Privacy Policy / プライバシーポリシー

**Researchmap Metrics** Chrome Extension

Last updated: 2026/5/19 (v1.14.20)

---

## 日本語

### 収集する情報

本拡張機能は、ユーザーの個人情報を一切収集しません。

### 外部送信

本拡張機能は、ユーザーに関する情報を外部サーバーに送信しません。

### データベースへのアクセス

本拡張機能は、ユーザーが researchmap の研究者ページを開いた際に、以下の公開データベースから、その研究者の論文に関する公開情報を取得します:

- [researchmap](https://researchmap.jp/) - 研究者公開ページ (HTML、論文メタデータ)
- [OpenAlex](https://openalex.org/) - 被引用数・著者ID・論文一覧（公開情報）
- [Crossref](https://www.crossref.org/) - 被引用数（公開情報）
- [ORCID](https://orcid.org/) - DOI情報（公開情報）
- [CiNii Research](https://cir.nii.ac.jp/) - 日本語論文DOI情報（公開情報）

これらのデータベースへのリクエストには、ユーザーの個人情報は含まれません（閲覧中のページの researchmap permalink、研究者の公開 ORCID、必要に応じて論文の DOI・タイトルのみが送信されます）。

**通信先ホスト**:
- researchmap.jp (デフォルトのデータ取得経路)
- api.openalex.org / api.crossref.org / pub.orcid.org / cir.nii.ac.jp
- api.researchmap.jp (上級設定で API 経路を有効化した場合のみ、要 JST 利用許諾)

### データ取得経路

デフォルトでは、researchmap の公開研究者ページの HTML を取得・解析する方式 (researchmap Web API 利用規約の適用外) を使用します。上級設定で Web API 経路に切り替えることができますが、その場合は JST から正式な利用許諾を得る必要があります。

### ローカルキャッシュ

計算結果は、Chromeブラウザのローカルストレージ（`chrome.storage.local`）に既定 168 時間 (1 週間、設定可能) 保存されます。これは、同じ研究者ページを再訪問したときに高速表示するためです。キャッシュは以下の場合に削除されます:

- 設定された有効期限経過後
- ユーザーが「再計算」ボタンをクリックしたとき
- データ取得経路を切り替えたとき (キャッシュフォーマット非互換のため)
- 拡張機能を削除したとき
- ユーザーが手動でChromeの拡張機能データを消去したとき

ローカルキャッシュはユーザーのローカルデバイスのみに保存され、外部に送信されることはありません。

### 問い合わせ

本プライバシーポリシーに関するお問い合わせは、拡張機能の開発者 (宮川 剛、藤田医科大学、ORCID: [0000-0003-0137-8200](https://orcid.org/0000-0003-0137-8200)、miyakawa@fujita-hu.ac.jp) まで。

---

## English

### Information Collected

This extension does not collect any personal information from users.

### External Transmission

This extension does not send any user-related information to external servers.

### Database Access

When the user opens a researcher page on researchmap, this extension retrieves publicly available information about that researcher's publications from the following databases:

- [researchmap](https://researchmap.jp/) - public researcher pages (HTML, paper metadata)
- [OpenAlex](https://openalex.org/) - citation counts, author IDs, work lists (public)
- [Crossref](https://www.crossref.org/) - citation counts (public)
- [ORCID](https://orcid.org/) - DOI information (public)
- [CiNii Research](https://cir.nii.ac.jp/) - Japanese paper DOI information (public)

These requests do not include any personal information about the user (only the researchmap permalink of the page being viewed, the researcher's public ORCID, and paper DOIs/titles as needed).

**Network hosts contacted**:
- researchmap.jp (default data source)
- api.openalex.org / api.crossref.org / pub.orcid.org / cir.nii.ac.jp
- api.researchmap.jp (only when API path is enabled via advanced settings; requires JST permission)

### Data Source

By default, the extension fetches and parses HTML from researchmap public researcher pages (outside the scope of the researchmap Web API Terms of Service). Users may opt into the Web API path via advanced settings, but doing so requires official permission from JST.

### Local Cache

Calculation results are stored in the Chrome local storage (`chrome.storage.local`) for a default of 168 hours (1 week, configurable) to enable fast display on subsequent visits. Cache is cleared when:

- The configured expiration period elapses
- User clicks the "Refresh" button
- The data source is switched (the cache format is incompatible across sources)
- The extension is uninstalled
- User manually clears Chrome extension data

The local cache is stored only on the user's local device and is never transmitted externally.

### Contact

For questions regarding this privacy policy, please contact the extension developer: Tsuyoshi Miyakawa (Fujita Health University, ORCID: [0000-0003-0137-8200](https://orcid.org/0000-0003-0137-8200), miyakawa@fujita-hu.ac.jp).
