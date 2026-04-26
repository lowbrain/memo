# ドメイン比較レポート (詳細解説版)

| 差分の分類 | @master-comment.md のドメイン | @update-comment.md のドメイン | ドメインの説明 | 変更・存在の理由 |
| :--- | :--- | :--- | :--- | :--- |
| **差なし** | *.manage.microsoft.com | *.manage.microsoft.com | コアサービスIntune | Intune管理通信の最重要エンドポイント（継続） |
| **差なし** | manage.microsoft.com | manage.microsoft.com | コアサービスIntune | Intune管理通信の最重要エンドポイント（継続） |
| **差なし** | *.dl.delivery.mp.microsoft.com | *.dl.delivery.mp.microsoft.com | コアサービスIntune | 配信の最適化（Delivery Optimization）に必須 |
| **追加** | - | *.dm.microsoft.com | コアサービスIntune | デバイス管理（Device Management）の標準ドメインとしての明文化 |
| **差なし** | *.do.dsp.mp.microsoft.com | *.do.dsp.mp.microsoft.com | コアサービスIntune | 配信の最適化サービス用（継続） |
| **差なし** | *.update.microsoft.com | *.update.microsoft.com | Windows Autopilotの依存関係 | Windows Update サービスの利用に必須 |
| **差なし** | *.windowsupdate.com | *.windowsupdate.com | Windows Autopilotの依存関係 | Windows Update サービスの利用に必須 |
| **差なし** | adl.windows.com | adl.windows.com | Windows Autopilotの依存関係 | Autopilotの診断および登録用 |
| **追加** | - | dl.delivery.mp.microsoft.com | コアサービスIntune | 配信の最適化ドメインの補完（ワイルドカードなし版の追加） |
| **差なし** | tsfe.trafficshaping.dsp.mp.microsoft.com | tsfe.trafficshaping.dsp.mp.microsoft.com | Windows Autopilotの依存関係 | 配信最適化のトラフィックシェーピング用 |
| **差なし** | time.windows.com | time.windows.com | Windows Autopilotの依存関係 | デバイスの時刻同期（NTP）に必須 |
| **差なし** | *.s-microsoft.com | *.s-microsoft.com | Windows Autopilotの依存関係 | 静的コンテンツ（CDN）提供用 |
| **差なし** | clientconfig.passport.net | clientconfig.passport.net | Windows Autopilotの依存関係 | Microsoft アカウント認証構成用 |
| **差なし** | windowsphone.com | windowsphone.com | Windows Autopilotの依存関係 | 歴史的経緯を含む登録用ドメインの維持 |
| **差なし** | approdimedatahotfix.azureedge.net | approdimedatahotfix.azureedge.net | PowerShell スクリプトと Win32 アプリ | アプリ配信CDN（継続、将来的に移行対象） |
| **差なし** | approdimedatapri.azureedge.net | approdimedatapri.azureedge.net | PowerShell スクリプトと Win32 アプリ | アプリ配信CDN（継続、将来的に移行対象） |
| **差なし** | approdimedatasec.azureedge.net | approdimedatasec.azureedge.net | PowerShell スクリプトと Win32 アプリ | アプリ配信CDN（継続、将来的に移行対象） |
| **差なし** | euprodimedatahotfix.azureedge.net | euprodimedatahotfix.azureedge.net | PowerShell スクリプトと Win32 アプリ | アプリ配信CDN（欧州リージョン用） |
| **差なし** | euprodimedatapri.azureedge.net | euprodimedatapri.azureedge.net | PowerShell スクリプトと Win32 アプリ | アプリ配信CDN（欧州リージョン用） |
| **差なし** | euprodimedatasec.azureedge.net | euprodimedatasec.azureedge.net | PowerShell スクリプトと Win32 アプリ | アプリ配信CDN（欧州リージョン用） |
| **差なし** | naprodimedatahotfix.azureedge.net | naprodimedatahotfix.azureedge.net | PowerShell スクリプトと Win32 アプリ | アプリ配信CDN（北米リージョン用） |
| **差なし** | naprodimedatapri.azureedge.net | naprodimedatapri.azureedge.net | PowerShell スクリプトと Win32 アアプリ | アプリ配信CDN（北米リージョン用） |
| **差なし** | naprodimedatasec.azureedge.net | naprodimedatasec.azureedge.net | PowerShell スクリプトと Win32 アプリ | アプリ配信CDN（北米リージョン用） |
| **差なし** | *.notify.windows.com | *.notify.windows.com | Windows プッシュ通知サービス (WNS) | デバイスへの通知・コマンドキック用 |
| **差なし** | *.wns.windows.com | *.wns.windows.com | Windows プッシュ通知サービス (WNS) | デバイスへの通知・コマンドキック用 |
| **差なし** | ekcert.spserv.microsoft.com | ekcert.spserv.microsoft.com | Windows Autopilotの依存関係 | ハードウェア構成証明（TPM）関連 |
| **差なし** | ekop.intel.com | ekop.intel.com | Windows Autopilotの依存関係 | Intel製チップのTPM証明書用 |
| **差なし** | ftpm.amd.com | ftpm.amd.com | Windows Autopilotの依存関係 | AMD製チップのTPM証明書用 |
| **差なし** | intunecdnpeasd.azureedge.net | intunecdnpeasd.azureedge.net | Android AOSPの依存関係 | Android管理用CDN |
| **差なし** | *.monitor.azure.com | *.monitor.azure.com | リモートヘルプ | 診断ログおよびモニタリング通信 |
| **差なし** | *.support.services.microsoft.com | *.support.services.microsoft.com | リモートヘルプ | サポートサービスとの通信 |
| **差なし** | *.trouter.communication.microsoft.com | *.trouter.communication.microsoft.com | リモートヘルプ | リアルタイム通信基盤（ACS）への接続 |
| **追加** | - | *.trouter.communications.svc.cloud.microsoft | リモートヘルプ | Microsoft サービスのドメイン集約（.cloud.microsoft）への対応 |
| **追加** | - | go-amer.trouter.communications.svc.cloud.microsoft | リモートヘルプ | 地域別通信エンドポイント（米州）の明文化 |
| **追加** | - | go-apac.trouter.communications.svc.cloud.microsoft | リモートヘルプ | 地域別通信エンドポイント（アジア）の明文化 |
| **追加** | - | go-eu.trouter.communications.svc.cloud.microsoft | リモートヘルプ | 地域別通信エンドポイント（欧州）の明文化 |
| **差なし** | *.trouter.teams.microsoft.com | *.trouter.teams.microsoft.com | リモートヘルプ | Teams通信基盤の利用 |
| **差なし** | api.flightproxy.skype.com | api.flightproxy.skype.com | リモートヘルプ | 機能フラグおよび構成管理用（レガシー互換維持） |
| **差なし** | ecs.communication.microsoft.com | ecs.communication.microsoft.com | リモートヘルプ | 構成設定取得サービス |
| **差なし** | edge.microsoft.com | edge.microsoft.com | リモートヘルプ | Edge基盤の共通通信用 |
| **差なし** | edge.skype.com | edge.skype.com | リモートヘルプ | リアルタイム通信のメディアリレー用 |
| **差なし** | remoteassistanceprodacs.communication.azure.com | remoteassistanceprodacs.communication.azure.com | リモートヘルプ | Azure Communication Services (ACS) への通信 |
| **差なし** | remoteassistanceprodacseu.communication.azure.com | remoteassistanceprodacseu.communication.azure.com | リモートヘルプ | ACSへの通信（欧州リージョン） |
| **差なし** | remotehelp.microsoft.com | remotehelp.microsoft.com | リモートヘルプ | リモートヘルプサービス本体 |
| **差なし** | wcpstatic.microsoft.com | wcpstatic.microsoft.com | リモートヘルプ | 静的コンテンツ（JS/CSS等）提供 |
| **差なし** | lgmsapeweu.blob.core.windows.net | lgmsapeweu.blob.core.windows.net | Windows Autopilotの依存関係 | リージョン別ストレージ（欧州） |
| **差なし** | intunemaape1.eus.attest.azure.net | intunemaape1.eus.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape10.weu.attest.azure.net | intunemaape10.weu.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape11.weu.attest.azure.net | intunemaape11.weu.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape12.weu.attest.azure.net | intunemaape12.weu.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape13.jpe.attest.azure.net | intunemaape13.jpe.attest.azure.net | デバイス正常性構成証明 | Azure Attestation（日本/アジア） |
| **差なし** | intunemaape17.jpe.attest.azure.net | intunemaape17.jpe.attest.azure.net | デバイス正常性構成証明 | Azure Attestation（日本/アジア） |
| **差なし** | intunemaape18.jpe.attest.azure.net | intunemaape18.jpe.attest.azure.net | デバイス正常性構成証明 | Azure Attestation（日本/アジア） |
| **差なし** | intunemaape19.jpe.attest.azure.net | intunemaape19.jpe.attest.azure.net | デバイス正常性構成証明 | Azure Attestation（日本/アジア） |
| **差なし** | intunemaape2.eus2.attest.azure.net | intunemaape2.eus2.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape3.cus.attest.azure.net | intunemaape3.cus.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape4.wus.attest.azure.net | intunemaape4.wus.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape5.scus.attest.azure.net | intunemaape5.scus.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape7.neu.attest.azure.net | intunemaape7.neu.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape8.neu.attest.azure.net | intunemaape8.neu.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | intunemaape9.neu.attest.azure.net | intunemaape9.neu.attest.azure.net | デバイス正常性構成証明 | Azure Attestation によるハードウェア整合性確認 |
| **差なし** | *.webpubsub.azure.com | *.webpubsub.azure.com | リモートヘルプ | Web PubSub 基盤を利用したリアルタイム通知 |
| **差なし** | *.gov.teams.microsoft.us | *.gov.teams.microsoft.us | リモートヘルプ | 政府用テナント（GCC High）向け互換ドメイン |
| **差なし** | remoteassistanceweb.usgov.communication.azure.us | remoteassistanceweb.usgov.communication.azure.us | リモートヘルプ | 政府用テナント向け ACS 通信 |
| **差なし** | config.edge.skype.com | config.edge.skype.com | コアサービスIntune | Edgeブラウザ管理用構成（継続） |
| **差なし** | fd.api.orgmsg.microsoft.com | fd.api.orgmsg.microsoft.com | コアサービスIntune | 組織内メッセージング機能用 |
| **差なし** | ris.prod.api.personalization.ideas.microsoft.com | ris.prod.api.personalization.ideas.microsoft.com | コアサービスIntune | パーソナライズ・提案機能用 |
| **追加** | - | *.powershellgallery.com | PowerShell スクリプトと Win32 アプリ | PowerShell モジュールのインストールに必須 |
| **追加** | - | cdn.oneget.org | PowerShell スクリプトと Win32 アプリ | PackageManagement (OneGet) のバックエンド |
| **追加** | - | go.microsoft.com | コアサービスIntune | 各種ツールへのリダイレクトに使用（最新ドキュメントでの明文化） |
| **追加** | - | aka.ms | コアサービスIntune | 短縮URL経由のダウンロード等に使用（最新ドキュメントでの明文化） |
| **追加** | - | displaycatalog.mp.microsoft.com | Microsoft Store | 新しい Microsoft Store (WinGet) アプリの検索 |
| **追加** | - | purchase.md.mp.microsoft.com | Microsoft Store | アプリのライセンス取得・購入処理 |
| **追加** | - | licensing.mp.microsoft.com | Microsoft Store | ライセンス検証サービス |
| **追加** | - | storeedgefd.dsx.mp.microsoft.com | Microsoft Store | ストアフロントのサービスエンドポイント |
| **追加** | - | *.events.data.microsoft.com | リモートヘルプ | 診断および利用状況データの送信（テレメトリ） |
| **差なし** | *.delivery.mp.microsoft.com | *.delivery.mp.microsoft.com | Windows Autopilotの依存関係 | コンテンツ配信基盤（DO） |
| **追加** | - | enterpriseregistration.windows.net | 認証の依存関係 | デバイスの Entra ID 登録に必須（依存関係の明確化） |
| **追加** | - | certauth.enterpriseregistration.windows.net | 認証の依存関係 | 証明書ベースのデバイス登録 |
| **追加** | - | login.microsoftonline.com | 認証の依存関係 | Microsoft Entra ID 認証の最重要エンドポイント |
| **追加** | - | graph.windows.net | 認証の依存関係 | デバイス情報参照のための Graph API 依存 |
| **追加** | - | config.office.com | 認証の依存関係 | Officeアプリの構成・デプロイ設定 |
| **追加** | - | ecs.office.com | コアサービスIntune | Office関連の構成設定サービス |
| **追加** | - | aadcdn.msauth.net | リモートヘルプ | 認証画面用静的リソース（CDN） |
| **追加** | - | aadcdn.msftauth.net | リモートヘルプ | 認証画面用静的リソース（CDN） |
| **追加** | - | browser.pipe.aria.microsoft.com | リモートヘルプ | 診断データ収集基盤（Aria） |
| **追加** | - | teams.microsoft.com | リモートヘルプ | Teamsとリモート操作アプリの連携統合 |
| **追加** | - | login.live.com | コアサービスIntune | コンシューマーアカウント認証用（最新での補完） |
| **追加** | - | lgmsapewus2.blob.core.windows.net | Windows Autopilotの依存関係 | リージョン別ストレージ（米国西部2） |
| **追加** | - | lgmsapesea.blob.core.windows.net | Windows Autopilotの依存関係 | リージョン別ストレージ（東南アジア） |
| **追加** | - | lgmsapeaus.blob.core.windows.net | Windows Autopilotの依存関係 | リージョン別ストレージ（オーストラリア） |
| **追加** | - | lgmsapeind.blob.core.windows.net | Windows Autopilotの依存関係 | リージョン別ストレージ（インド） |
| **削除** | *.prod.do.dsp.mp.microsoft.com | - | Windows Autopilotの依存関係 | `*.do.dsp.mp.microsoft.com` への集約による整理 |
| **削除** | swda01-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swda02-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アアプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swdb01-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swdb02-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swdc01-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swdc02-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swdd01-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アアプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swdd02-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swdin01-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アアプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | swdin02-mscdn.azureedge.net | - | PowerShell スクリプトと Win32 アプリ | 2025年3月のCDNドメイン移行に伴う廃止 |
| **削除** | *.emdl.ws.microsoft.com | - | コアサービスIntune | アプリ配信基盤の刷新とドメイン整理 |
| **削除** | *.itunes.apple.com | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | *.mzstatic.com | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | *.phobos.apple.com | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | 5-courier.push.apple.com | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | ax.itunes.apple.com.edgesuite.net | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | itunes.apple.com | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | ocsp.apple.com | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | phobos.apple.com | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | phobos.itunes-apple.com.akadns.net | - | Apple デバイス管理 | Intuneコアリストから特定プラットフォーム用リストへ分離 |
| **削除** | *.trouter.skype.com | - | リモートヘルプ | Skype基盤からACS（Azure Communication Services）への完全移行 |
| **削除** | contentauthassetscdn-prod.azureedge.net | - | PowerShell スクリプトと Win32 アアプリ | 旧CDNドメインの廃止・集約 |
| **削除** | contentauthassetscdn-prodeur.azureedge.net | - | PowerShell スクリプトと Win32 アアプリ | 旧CDNドメインの廃止・集約 |
| **削除** | contentauthrafcontentcdn-prod.azureedge.net | - | PowerShell スクリプトと Win32 アアプリ | 旧CDNドメインの廃止・集約 |
| **削除** | contentauthrafcontentcdn-prodeur.azureedge.net | - | PowerShell スクリプトと Win32 アプリ | 旧CDNドメインの廃止・集約 |
