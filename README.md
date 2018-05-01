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

# INSTALANDO O DEVISE

	* adicione ao seu gem file a seguinte linha: gem 'devise'
	* bundle install
	* rails generate devise:install

# CONFIGURE O AMBIENTE
	
	* No diretorio config/environments/development.rb, adicione a linha :
		Rails.application.configure do
 		
 			 config.action mailer.default url options = { host: 'localhost', port: 3000 }


# DATABASE

	* rails generate devise User

# CONTROLLERS
	
	* Adicione o helper nos seus controllers para que o devise verifique a autenticação do usuario

		before_action :authenticate_user!

# VIEW

	* No arquivo config/initializers/devise.rb descomente e midifique a seguinte linha:
		
		config.scoped_views = true

	* No terminal execute: rails generate devise:views users

