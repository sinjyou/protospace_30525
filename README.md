##  usersテーブル

## users テーブル

| Column     | Type   | Options  |
| ---------- | ------ | -------- | 
| email      | string | NOT NULL |
| password   | string | NOT NULL |
| name       | string | NOT NULL |
| profile    | text   | NOT NULL |
| occupation | text   | NOT NULL |
| position   | text   | NOT NULL |

## prototype テーブル

| Column     | Type               | Options     |
| ---------- | ------------------ | ----------- |
| title      | string             | NOT NULL    |
| catch_copy | text               | NOT NULL    |
| concept    | text: false        | NOT NULL    |
| image      | ActiveStorageで実装 |             |
| user       | references         |             |

## comments テーブル

| Column    | Type      | Options     |
| --------- | --------  | ------------|
| text      | text      | NOT NULL    |
| user      | reference |             |
| prototype | reference |             |

