source 'https://rubygems.org'

Encoding.default_external = Encoding::UTF_8
Encoding.default_internal = Encoding::UTF_8

gem 'rails', '~> 4.1'
gem 'pg', '~> 0.17'
gem 'devise'
gem 'paperclip', '~> 4.2'
gem 'ckeditor'
gem 'friendly_id', '~> 5.0.0'
gem 'will_paginate', '~> 3.0'
gem 'ancestry'
gem 'jquery-rails'
gem 'jquery-ui-rails'
gem 'nokogiri'
gem 'airbrake'
gem 'nested_form', '0.3.1'
gem 'spreadsheet', '0.6.5.3' # why? and why this old version?
gem 'rack', '1.5.2'
gem 'hpricot', '~> 0.8.4'
gem 'recaptcha', '0.3.4', :require => 'recaptcha/rails'
gem 'cancancan'
gem 'draper'
gem 'sass-rails', '~> 5.0.0'
gem 'font-awesome-sass'
gem 'compass-rails', '~> 2.0.4'
gem 'susy'
gem 'pg_search'
gem 'sitemap_generator'
gem 'whenever'
gem 'httparty'
gem 'uglifier'

# Use unicorn for serving the app on AWS
group :staging, :staging_published, :production, :production_published do
  gem 'unicorn'
end

group :development, :development_published, :test do
  gem 'shoulda-matchers'
  gem 'rake'
  gem 'thin'
  gem 'cucumber-rails', :require => false
  gem 'database_cleaner' # database_cleaner is not required, but highly recommended
  gem 'rspec-rails'
  gem 'rspec-its'
  gem 'rspec-activemodel-mocks'
  gem 'rspec-collection_matchers'
  gem 'spork'
  gem 'launchy'    # So you can do Then show me the page
  gem 'autotest-rails'
  gem 'factory_girl_rails'
  gem 'faker'
  gem 'ZenTest'
  gem 'escape_utils' # Fixes Rack issue when UTF-8 strings are sent in the params
  gem 'columnize'
  gem 'pry-rails'
  # gem 'pry-byebug'
  # gem 'byebug'
end

group :development, :development_published do
  gem 'wirble'
  gem 'hirb'
  gem 'rails3-generators'
  gem 'railroady'
end
