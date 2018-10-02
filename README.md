RUBY
========

DOCS : https://www.ruby-lang.org/fr/libraries/
TUTO : https://guides.rubyonrails.org/getting_started.html
Config: https://guides.rubyonrails.org/configuring.html

Prerequisite:
========
What you need to make Ruby work
- Unix		OS (Debian / Ubuntu)
- Gem		package manager for ruby
- Rails		ruby framework for devs 
- NodeJS		Package manager for JS
- Apache2
- Mysql database
- PhpMyAdmin

Gems
========
Gem is the package manager for ruby, it provides a lot of modules for ruby application such as Rails
https://rubygems.org/

NodeJS:
========
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

Process:
========
Download client mysql for ruby (connector):

`sudo apt-get install python-dev default-libmysqlclient-dev`

Then install mysql2 via gem too enable mysql connection with ruby application

`gem install mysql2`

Create DB and populate tables

`rake db:create`

`rake db:migrate`

