source 'http://rubygems.org'

# Backend
gem 'rails', '~> 3.2.21'
gem 'mysql2', '~> 0.3.10'
gem 'devise', '3.0.1'
gem 'ckeditor'
gem 'carrierwave'
gem 'mini_magick', '3.6.0'
gem 'will_paginate', '3.0.5'
gem 'has_publishing'
gem 'dynamic_form'
gem 'nested_form'
gem 'strong_parameters'
gem 'ransack'
gem 'dalli'
gem 'delayed_job_active_record'
gem 'daemons'
gem 'rubyzip'

# Frontend
gem 'jquery-rails'
gem 'chosen-rails'
gem 'kaminari'
gem 'bootstrap-kaminari-views'

# We have to use the git version of Prawn because they are useless at
# actually releasing gem versions consistently.
# The reason we need such a bleeding-edge version of Prawn is for
# colspan and rowspan support.
# FIXME: Use gem version of Prawn once once gets released with
# colspan support.
gem 'prawn', :git => 'https://github.com/prawnpdf/prawn.git', :ref => '2d40e4d73270a1e6a2a294aec12f5705a52969e6'

#Analytics
gem 'google-analytics-rails'
gem 'twitter-bootstrap-rails'
gem 'bootstrap-datepicker-rails'

# Gems used only for assets and not required
# in production environments by default.
group :assets do
  gem 'sass-rails',   '~> 3.2.3'
  gem 'coffee-rails', '~> 3.2.1'
  gem 'less-rails'

  # See https://github.com/sstephenson/execjs#readme for more supported runtimes
  gem 'therubyracer', '0.12.0', :platforms => :ruby

  gem 'uglifier', '>= 1.0.3'
end

group :development, :test do
  gem 'thin'
  gem 'shoulda'
  gem 'rspec-rails'
  gem 'factory_girl_rails'
  gem 'faker'
  gem 'capistrano'
  gem 'rvm-capistrano', require: false
  gem 'capistrano-ext'
  gem 'rb-fsevent'
  gem 'pry'
end

group :test do
  gem 'database_cleaner'
  gem 'guard-bundler'
	gem 'capybara'
  gem 'poltergeist'
  gem 'spork-rails'
  gem 'guard-spork'
  gem 'guard-rspec'
  gem 'launchy'
  gem 'simplecov'
end
