# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## 環境構築
1. git clone 
2. gemfileに 追記　
gem "cssbundling-rails"

gem 'importmap-rails'
gem 'propshaft'


3. docker-compose run web rails new . --force --no-deps --database=mysql --css sass
4. dc exec web bundle install
5. dc run web bin/rails importmap:install
6. dc build --no-cache   (bundle installしたらこれする)
7. npm install bootstrap
8. npm i bootstrap-icons
