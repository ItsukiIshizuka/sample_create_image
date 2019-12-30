# README

## gem list
* pry-rails
* jquery-rail https://github.com/rails/jquery-rails
* haml-rails https://github.com/haml/haml-rails
* carrierwave 

## 構築手順
* productテーブル作成(name:string)
* imageテーブル作成(name:string, product_id:外部キー)
* 親 productモデル 子 imageモデル で構築
* "carrierwave"導入後、以下のコードを実行

```
rails g uploader images
```
* image モデルに以下の一文を追加

```
mount_uploader :name, ImagesUploader
```
* 画像のアップロードテスト

## What
* fields_forを用いた複数モデルの登録(ProductとImageテーブル)

## Why
* メルカリ技術の細分化

## 参考記事
* fields_forを用いた画像のアップロード https://qiita.com/kouuuki/items/5daf2b5f34273d8457f7
* 

