# Entra connect 導入のヒント

## 1.必要な実装（キーワード）
- パスワードハッシュ同期
- セルフパスワードリセット
- パスワードライトバック
- シングルサインオン
- Microsoft Entra ハイブリッド参加（対象範囲はAVDのみ）

## 2.Entra Connectのインストール（パスワードハッシュ同期）
### 前提条件
https://learn.microsoft.com/ja-jp/entra/identity/hybrid/connect/how-to-connect-install-prerequisites

### インストール
https://learn.microsoft.com/ja-jp/entra/identity/hybrid/connect/how-to-connect-install-express

### インストール後
https://learn.microsoft.com/ja-jp/entra/identity/hybrid/connect/how-to-connect-post-installation

### 補足
- 同期の対象範囲を限定したい場合は、インストール後において [フィルター処理](https://learn.microsoft.com/ja-jp/entra/identity/hybrid/connect/how-to-connect-sync-configure-filtering) なる対応を考慮
- [カスタムインストール](https://learn.microsoft.com/ja-jp/entra/identity/hybrid/connect/how-to-connect-install-custom) を用いれば、インストールのタイミングで以下設定が可能
  - フィルター処理
  - パスワードライトバック
  - シングルサインオン

## 3.セルフパスワードリセット（パスワードライトバック含む）の有効化
https://learn.microsoft.com/ja-jp/entra/identity/authentication/tutorial-enable-sspr-writeback

## 4.シングルサインオンの有効化
https://learn.microsoft.com/ja-jp/entra/identity/hybrid/connect/how-to-connect-sso-quick-start

## 5.Microsoft Entra ハイブリッド参加（対象範囲はAVDのみ）の構成


