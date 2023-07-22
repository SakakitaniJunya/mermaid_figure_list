# Python Web GetPost HttpRequest

## 送受信処理
- Get：メッセージ受信
- Post：メッセージ送信

```mermaid
sequenceDiagram
    participant ユーザー as User
    participant ブラウザ as Browser
    participant サーバー as Fllask Server
    participant データベース as SQLite

    Loop every 5 milliseconds
        ユーザー->>ブラウザ: ページを開く
        ブラウザ->>サーバー: HTTP GETリクエスト
        サーバー->>データベース: SQLクエリ
        データベース-->>サーバー: クエリ結果
        サーバー-->>ブラウザ: HTTPレスポンス（HTML）
        ブラウザ-->>ユーザー: ページを表示
    End
    
    ユーザー->>ブラウザ: フォームを送信
    ブラウザ->>サーバー: HTTP POSTリクエスト（フォームデータ）
    サーバー->>データベース: SQLクエリ（データの挿入/更新）
    データベース-->>サーバー: クエリ結果
    サーバー-->>ブラウザ: HTTPレスポンス（リダイレクトまたは更新されたページ）
    ブラウザ-->>ユーザー: 更新されたページを表示

```