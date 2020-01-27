# クラス図

## goals
目標のツイート

| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| mr_content | text |
| an_content | text |
| cp_content | text |
| user_id | integer |
| created_at | datetime |
| updated_at | datetime |


## users
サービスを使うユーザー

| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| name | string |
| email | string |
| image | string |
| introduction | text |
| created_at | datetime |
| updated_at | datetime |
| password_digest | string |
| remember_digest | string |
| admin | boolean |
| activation_digest | string |
| activated | boolean |
| activated_at | datetime |
| reset_digest | string |
| reset_sent_at | datetime |

## relationships
フォローフォロワー

| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| follower_id | integer |
| followed_id | integer |
| created_at | datetime |
| updated_at | datetime |


## categories
カテゴリー

| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| name | string |
| created_at | datetime |
| updated_at | datetime |

## goal_category_relations
ツイートとカテゴリーを繋ぐテーブル

| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| goal_id | integer |
| category_id | integer |
| created_at | datetime |
| updated_at | datetime |


## likes
ツイートのいいね

| カラム名 | 型 |
|:-----------|:------------|
| user_id | integer |
| goal_id | integer |

## comments
ツイートのコメント

| カラム名 | 型 |
|:-----------|:------------|
| user_id | integer |
| goal_id | integer |
| content | text |
