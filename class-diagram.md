# クラス図

## goals
| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| m_content | text |
| v_content | text |
| c_content | text |
| user_id | integer |
| created_at | datetime |
| updated_at | datetime |


## users
| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| name | string |
| email | string |
| icon | string |
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
| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| follower_id | integer |
| followed_id | integer |
| created_at | datetime |
| updated_at | datetime |


## categories
| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| name | string |

## goal_category_relations
| カラム名 | 型 |
|:-----------|:------------|
| id | integer |
| goal_id | integer |
| category_id | integer | 


## likes
| カラム名 | 型 |
|:-----------|:------------|
| user_id | integer |
| goal_id | integer |

## comments
| カラム名 | 型 |
|:-----------|:------------|
| user_id | integer |
| goal_id | integer |
| content | text |
