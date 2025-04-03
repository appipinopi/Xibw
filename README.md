# Xibw Bot

Xibw Botは、X（旧Twitter）APIと連携したDiscord Botです。Xのアカウントやハッシュタグのデータをリアルタイムで取得し、Discordに通知する機能を提供します。また、YouTube、Instagram、Twitchのリンクにも対応し、関連情報を自動で取得して投稿します。

## 機能一覧
- **X API連携**: Xアカウント、ハッシュタグ、フォロワー、リポストの監視
- **YouTubeリンク対応**: YouTubeリンクを自動的に認識して処理
- **Instagramリンク対応**: Instagramリンクを自動的に認識して処理
- **Twitchリンク対応**: Twitchリンクを自動的に認識して処理
- **Discord Bot**: コマンドを使ってAPIの状態やエラーを確認可能
- **自動API更新機能**: 60秒ごとにX APIをチェックし、Tweepyのバージョンも毎日確認

## 必要なもの
- **Deno Deploy**: Deno環境でホスティング
- **GitHub**: リポジトリ管理
- **Discord Bot Token**: Discordにボットを追加するためのトークン
- **X APIキー**: X（Twitter）APIのアクセス認証情報
- **環境変数**: Botの動作に必要な認証情報を環境変数で設定

## コマンド

- **`/status`**: APIの状態を手動で確認  
- **`/X [user/u] [username/@/URL] [class]`**: Xアカウントを登録  
- **`/X [hash/h] [word] [class]`**: Xハッシュタグを登録  
- **`/X [start/sa] [ALL/class]`**: APIの自動更新を開始  
- **`/X [stop/so] [ALL/class]`**: APIの自動更新を停止  
- **`/X [delete/d] [class]`**: 登録したユーザー、ハッシュタグを削除

## デプロイ後の動作確認
- Discord Botが正常に起動しているか確認  
- APIエラー発生時にDiscord通知が届くことを確認

## 注意事項
- **配布は行っていません**。このBotはhttps://discord.com/oauth2/authorize?client_id=1356841089193087016 から利用はできます。
---
