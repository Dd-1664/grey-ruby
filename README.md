RUBY
========

DOCS : https://www.ruby-lang.org/fr/libraries/

TUTO : https://guides.rubyonrails.org/getting_started.html

Config: https://guides.rubyonrails.org/configuring.html

# Prerequisite:

What you need to make Ruby work
- Unix		OS (Debian / Ubuntu)
- Gem		package manager for ruby
- Rails		ruby framework for devs 
- NodeJS		Package manager for JS
- Apache2
- Mysql database
- PhpMyAdmin

# Gems

Gem is the package manager for ruby, it provides a lot of modules for ruby application such as Rails

https://rubygems.org/

# NodeJS:

Node JS is required to execute Javascript code in ruby application (JS manger + interpreter)
Its’s needed to execute command in CLI from Rails.

`curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash –`

`sudo apt-get install -y nodejs`

Database:
========
By Default Ruby use mysqlite3, to use MySQL in Ruby On Rails:

https://www.digitalocean.com/community/tutorials/how-to-use-mysql-with-your-ruby-on-rails-application-on-ubuntu-14-04

https://pypi.org/project/mysqlclient/

https://www.1and1.com/cloud-community/learn/application/ruby-on-rails/how-to-use-mysql-with-your-ruby-on-rails-application/

# Process:

Download client mysql for ruby (connector):

`sudo apt-get install python-dev default-libmysqlclient-dev`

Then install mysql2 via gem too enable mysql connection with ruby application.

Fill /config/database.yml with DB credentials.

`gem install mysql2`

Create DB and populate tables.

`rake db:create`

`rake db:migrate`

# Rename App

http://www.adamscott.io/blog/2014/01/21/renaming-a-ruby-on-rails-application/

# Install Devis

https://rubygems.org/gems/devise

- Add this to Gemfile:

`gem 'devise', '~> 4.5'`

- Then install it:

`bundle install`

- Add devise to your application

`rails generate devise:install`

- After, follow process on terminal.

- Then generate views for Login & Signup page.

`rails generate devise:views`

- Create a User, access to this page.
`http://[IPv4_ADDR]:3000/users/sign_up`

# WARNING:
IF TABLE USERS IS CREATED, DO NOT MIGRATE
migration stored in:
`/db/migration`
