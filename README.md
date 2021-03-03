
## users テーブル

| Column     | Type   | Options     |
| --------   | ------ | ----------- |
| email      | string | null: false |
| password   | string | null: false |
| name       | string | null: false |
| profile    | text   | null: false |
| occupation | text   | null: false |
| postion    | text   | null: false |



## comments テーブル

| Column     | Type       | Options      |
| ---------- | ---------- | -------------|
| text       | text       | null: false  |
| user       | references |              |
| prototype  | references |              |

## prototypes テーブル

| Column     | Type         | Options       |
| ---------- | ------------ | --------------|
| title      | string       | null: false   |
| catch_copy | text         | null: false,  |
| concept    | text         | null: false,  |
| image      | ActiveStrage |               |
| user       | references   |               |