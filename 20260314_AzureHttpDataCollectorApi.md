## 【重要】Azure Log Analytics（Sentinel）データ転送方式の廃止と移行に関する報告

現在 Netskope から Azure Sentinel へのログ転送に使用している **「HTTP Data Collector API」** は、Microsoft の公式スケジュールに基づき、**2026年9月14日**に廃止されます。

これに伴い、認証に使用している **「プライマリ キー（共有キー）」** を用いた接続も利用できなくなります。

### 1. 廃止の事実と根拠（公式アナウンス）

Microsoft は、セキュリティ強化のため、従来の共有キー認証を廃止し、新しい「ログ インジェスト API」へ移行することを公式に通知しています。

* **廃止対象:** HTTP Data Collector API
* **廃止期限:** **2026年 9月 14日**
* **公式アナウンス (Azure 更新情報):**
* **[Azure Monitor データ コレクター API の廃止（公式 Update）](https://azure.microsoft.com/ja-jp/updates/?id=azure-monitor-data-collection-api-retirement)**


> ※このページにて「2026年9月14日までに、ログ インジェスト API を使用するようにスクリプトを更新してください」と明記されています。


* **技術解説・移行ガイド (Microsoft Learn):**
* [HTTP データ コレクター API からログ インジェスト API に移行する](https://learn.microsoft.com/ja-jp/azure/azure-monitor/logs/custom-logs-migrate)
* [2026 年のサポート終了予定（Azure Monitor データ コレクター API）](https://learn.microsoft.com/ja-jp/lifecycle/end-of-support/end-of-support-2026)



### 2. Netskope 連携への直接的な影響

調査の結果、現在参照している Netskope の設定ドキュメント（[Log Shipper Plugin](https://docs.netskope.com/en/microsoft-azure-sentinel-plugin-for-log-shipper)）は、この廃止対象の仕組みを利用しています。

* **認証方式:** `Workspace ID` と **`Primary Key`** を使用。
* **データ構造:** 送信先が `_CL`（カスタム ログ）テーブル。
* **リスク:** 2026年9月14日以降、この API エンドポイントが閉鎖され、Netskope からのログ転送が**完全に遮断**されます。

### 3. 移行先：Logs Ingestion API（ログ インジェスト API）

今後は、プライマリ キーに依存しない、Microsoft Entra ID（旧 Azure AD）による認証への移行が必要です。

* **新しい認証:** **Microsoft Entra ID の「アプリ登録」** によるトークン認証。
* **新しい構成要素:** Azure 側に **「データ収集ルール (DCR)」** と **「データ収集エンドポイント (DCE)」** を新たに作成し、ログの受け口を再定義します。
* **詳細ガイド:**
* [ログ インジェスト API の概要](https://learn.microsoft.com/ja-jp/azure/azure-monitor/logs/logs-ingestion-api-overview)



### 4. まとめと推奨アクション

廃止まで半年を切っており、インフラ側のリソース設計（DCR/DCE）と Netskope 側のプラグイン設定変更が必要になるため、早期の着手を推奨します。

1. **現状特定:** Netskope 管理画面にて、実際に「Primary Key」が設定されている箇所を特定。
2. **ベンダー（Netskope）への確認:** 2026年9月の API 廃止に対応した、最新の「DCR 対応プラグイン」への移行手順を確認。
3. **検証環境の構築:** 新しい認証方式（アプリ登録）および DCR の作成・テスト。

**この資料を共有する際、チームメンバーから「今の設定をそのまま新 API に流用できるか？」といった技術的な質問が出るかもしれません。そのあたりの補足が必要であれば、いつでもお伝えします。**
