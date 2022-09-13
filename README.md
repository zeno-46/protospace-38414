usersテーブル
| column             |  type  |  options
| ------------------ |--------|----------
| email              | string | NOT NILL,ユニーク制約
| encrypted_password | string | NOT NULL
| name               | string | NOT NULL
| profile            | text   | NOT NULL
| occupation         | text   | NOT NULL
| position           | text   | NOT NULL

prototypesテーブル
| column             |  type     |  option
|--------------------|--------   |----------
| title              | text      | NOT NULL
| catch_copy         | text      | NOT NULL
| concept            | text      | NOT NULL
| user               |references | NOT NULL,外部キー

commentsテーブル
| column             |  type     |  option
|--------------------|-----------|-----------
| content            | text      | NOT NULL
| prototype          | references| NOT NLL,外部キー
| user               | references| NOT NULL,外部キー