source 'https://rubygems.org'

gem 'rails', '~> 4.1.13'

# Use postgresql as the database for Active Record
gem 'pg'

# Use resque for managing Resque queues
# TODO: migrater to ActiveJob pattern after upgrading to Rails 4.2
gem 'resque'

# Use resquemailer for queueing emails
gem 'resque_mailer'

# Use resque-scheduler to schedule tasks
gem 'resque-scheduler'

# Use redis-store for caching on Rails
gem 'redis-rails'

# use draper to start using decorators
gem 'draper', '~> 1.3'

# Notify of exceptions to our Airbrake account
gem 'airbrake'

# Load settings from .env into ENV
gem 'dotenv-rails'

# Use SCSS for stylesheets
gem 'sass-rails', '5.0.4'

# Use bootstrap for admin styles
gem 'bootstrap-sass'

# Use fontawesome for nice icons
gem 'font-awesome-sass-rails'

# Use foundation for the public facing styles
# TODO: There's a bug inside the foundation form.js
# it's simple enough that it should get merged but we are depending
# on a fork for now.
gem 'zurb-foundation', git: "git@github.com:3months/foundation.git"

# Use select2 for a better multiselect interface
gem 'select2-rails'

# Use sortable for positioning content blocks
gem 'jquery-ui-rails', '~> 5.0.5'

# TODO peer-review use of this gem
gem "bootstrap-sass-extras", "0.0.6" # Bootstrap SASS extras includes some helpers and generators to speed up templating

# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '~> 2.7'

# Use CoffeeScript for .js.coffee assets and views
gem 'coffee-rails', '~> 4.1.0'

# See https://github.com/sstephenson/execjs#readme for more supported runtimes
gem 'therubyracer', platforms: :ruby
gem 'libv8', '3.16.14.7'

# Use jquery as the JavaScript library
gem 'jquery-rails'

# Use jquery cookie plugin
gem 'jquery-cookie-rails', '~> 1.3.1.1'

# Use jquery multi part plugin
gem 'remotipart', '~> 1.2'

# Use recaptcha to fend off baddies for member and admin logins
gem 'recaptcha', require: 'recaptcha/rails'

# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2'

# Authentication for administrators and members with devise
gem 'devise'

# Authorization with cancan
gem 'cancan', :git => 'https://github.com/3months/cancan', :branch => 'strong_parameters'

# Use FriendlyId for generating slugs
gem 'friendly_id', :git => 'https://github.com/FriendlyId/friendly_id.git'

# Tagging
gem 'acts-as-taggable-on', '~> 3.0.2'

# Markdown parsing
gem 'redcarpet'

# HTML to markdown for exporting product xml
gem 'reverse_markdown'

# TODO revert back to gem version once stable release for Rails 4 is released
# TODO currently waiting to hear about fix to papertrail to work with
## acts-as-taggable-on: https://github.com/airblade/paper_trail/pull/236
gem 'paper_trail', :git => 'https://github.com/3months/paper_trail.git', :branch => 'rails4' # Use PaperTrail for audit log + snapshots

# Use Kaminari for pagination
gem 'kaminari'

# Upload assets to s3
gem 'fog', '~> 1.32.0'
# Assets en S3
gem 'asset_sync'

# Carrierwave handles file uploads in a really nice way
gem 'carrierwave'
# for deferring carrierwave image processing.
gem 'carrierwave_backgrounder'
# lossless optmize images
gem 'carrierwave-imageoptimizer'

# ...but requires mini_magick to perform resizing, etc.
gem 'mini_magick'

# Use Flex as our wrapper around ElasticSearch server
gem 'rest-client'
gem 'flex-rails'

# Use Nokogiri for reading and processing product import files
gem 'nokogiri'

# Use ransack for filtering and sorting
gem "ransack"

# Add a 'country select' helper using ISO-3166
gem 'country_select'

# Make payments to DPS PxPay
gem 'pxpay'

# Force a working version of savon to use with pxfusion. Temporary.
gem 'savon', '~> 2.5.1'

# Make refunds from DPS PxPost using the activemerchant gem
gem 'activemerchant'

# Allow required pages to be accessed with first click free (FCF)
gem 'first_click_free'

# Barcode generation
gem 'barby'

# PDF generation
gem 'prawn', '~> 1.0.0'

# Control the date-time continuum
gem 'timecop'

# Utility gem to remove default_scope on association
gem 'unscoped_associations'

# Use useragent for parsing the HTTP_USER_AGENT
gem 'useragent'

# Use hashie for powerful object like hashes
gem 'hashie'

# Whenever handles crontab management
gem 'whenever', require: false

gem 'newrelic_rpm'

group :doc do
  # bundle exec rake doc:rails generates the API under doc/api.
  gem 'sdoc', require: false
end

# emails css
group :production, :production_published, :staging, :staging_published do
  gem 'premailer-rails'
end

group :development, :development_published, :test, :test_published do

  # RSpec makes testing nicer
  gem 'rspec-rails', '~> 2.14.2'

  # Factories make tests simpler
  gem 'factory_girl_rails'

  # Use Capistrano for deployment
  gem 'capistrano', '~>2.15.7'

  # Cap control of remote Resque workers
  gem "capistrano-resque"

  # Use livereload to help with front end development speed
  gem 'guard-livereload',        :require => false
  gem 'rack-livereload'

  gem 'guard-rspec',        :require => false

  # Use smacssify to quickly setup a SCSS folder structure
  gem 'smacssify'
end

group :test, :test_published do
  # Integration tests use cucumber
  gem 'cucumber-rails', require: false

  # Browser tests are driven by capybara
  gem 'capybara'

  # Use phantomjs to drive javascript integration tests
  gem 'poltergeist'

  # Clean test database with database_cleaner
  gem 'database_cleaner'

  # Easily asset model behaviours
  gem 'shoulda', :require => false
  gem 'shoulda-matchers', :require => false

  # Save and open pages to debug tests
  gem 'launchy'

  # Stub and mock HTTP request
  gem 'webmock', '~>1.11.0'

  # Leverage webmock to store and replay HTTP requests
  gem 'vcr'

end

# gem 'debugger', group: [:development, :test, :development_published, :test_published]
# gem 'byebug', group: [:development, :test, :development_published, :test_published]
gem 'pry', group: [:development, :test, :development_published, :test_published]
# gem 'certified', group: [:development, :development_published]
# gem 'pry-byebug', group: [:development, :test, :development_published, :test_published]
