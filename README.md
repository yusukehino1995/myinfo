## usersテーブル

|Column|Type|Options|
|------|----|-------|
|email|text|null: false|
|password|string|null: false|

### Association
- has_many :addresses
- has_many :routes
- has_many :keywords

## addressesテーブル

|Column|Type|Options|
|------|----|-------|
|address|text|null: false, index: true|

### Association
- belongs_to user

## routesテーブル

|Column|Type|Options|
|------|----|-------|
|route|integer|null: false, index: true|

### Association
- belongs_to :user

## keywordsテーブル

|Column|Type|Options|
|------|----|-------|
|keyword|text|null: true, index:true|

### Association
- belongs_to :user
