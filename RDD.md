# サービスの要件定義

## 画面遷移
### 新規登録・ログイン
- ホーム→ログインor新規登録→ログイン後のホーム

### 目標登録
- ホーム→目標登録→登録した目標の詳細

### その他
- ホーム→プロフィール→プロフィール編集
- ホーム→カテゴリ検索
- ホーム→キーワード検索
- ホーム→目標詳細

## 機能設計
### トップ(ログイン前)
処理内容:

 - DBから目標情報を取得
 - 目標情報を画面に表示
 - 各ページへのリンクを表示

必要なデータ:

 - 目標情報、ユーザー情報

取得元:

 - DBから取得

操作:

 - ログイン、新規登録、検索、詳細をクリック

### トップ(ログイン後)
処理内容

- DBから目標情報を取得
- 目標情報を画面に表示
- 各ページへのリンクを表示

必要なデータ:

- 目標情報、ユーザー情報
取得元:

- DBから取得

操作:

- 検索、詳細をクリック

### カテゴリ検索
処理内容:

- ドロップダウンのカテゴリの中から、カテゴリを受け取る検索条件をもとに、dbから目標検索

必要なデータ:

- 目標情報

取得元:

- 画面入力

操作:

- ドロップダウンメニューから選ぶ→検索を押す

### キーワード検索
処理内容:

 - フォームから検索条件を受け取る。検索条件をもとにdbから目標検索

必要なデータ:

 - 目標情報、ユーザー情報

取得元:

 - 画面入力

操作:

 -フォームに入力→検索をクリック

### マイページ
処理内容:

 - DBからユーザー情報を取得
 - ユーザー情報を画面に表示
 - リンクを表示

必要なデータ:

 - ユーザー情報
取得元:

 - DBから取得
操作:

 - ログアウト
 - プロフィール編集
 - 目標詳細
 - 編集

### 目標登録機能
処理内容:

 - ユーザーの目標をDBに登録

必要なデータ:

 - 目標情報

取得元:

 - 画面入力

操作:

 - 目標内容を記入→送信ボタンを押す

### 目標詳細表示機能
処理内容:

 - ユーザーの詳細な目標を表示
 - いいね数、コメントを表示フォロー

必要なデータ:

 - 目標情報
取得元:

 - DBから取得

操作:

 - いいね
 - コメント
 - フォロー

### ログイン機能
処理内容:

 - 入力フォームから情報を受け取る
 - 合っていればユーザーがログイン
必要なデータ:

 - ユーザー情報
取得元:

 - 入力フォーム
操作:

 - フォームに入力→ログインボタンを押す

### 新規登録機能
処理内容:

 - 入力フォームから情報を受け取るユーザー情報をデータベースに保存
必要なデータ:

 - ユーザー情報
取得元:

 - 入力フォーム
操作:

 - フォームに入力→登録ボタンを押す

### プロフィール編集機能
処理内容:

 - DBからユーザー情報を取得
 - ユーザー情報を画面に表示入力所フォームから新たな情報を受け取るパスワードがあっていれば変更

 必要なデータ:

 - ユーザー情報
取得元:

 - DBと、フォームから取得
操作:

 - フォームに入力→登録を押す

## データベース設計
### ユーザーマスタ
**ユーザー ID**
- メールアドレス
- パスワード
- 名前
- 画像
- 性別
- 年齢
- 職業
- コメント
- フォロー
- フォロワー

### 目標マスタ
**目標ID**
- Mの項目
- Aの項目
- Cの項目
- カテゴリ
- 目標登録日時
- いいね
- コメント
