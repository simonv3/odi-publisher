source 'https://rubygems.org'
source 'https://BnrJb6FZyzspBboNJzYZ@gem.fury.io/govuk/'

#ruby=ruby-1.9.3
#ruby-gemset=quirkafleeg-publisher

gem 'dotenv-rails'

gem 'aws-ses', require: 'aws/ses'

if ENV['BUNDLE_DEV']
  gem 'gds-sso', path: '../gds-sso'
else
  gem 'gds-sso', '9.2.2'
end

gem "govuk_content_models", '6.1.0'

if ENV['CONTENT_MODELS_DEV']
  gem "odi_content_models", path: '../odi_content_models'
else
  gem "odi_content_models", :github => 'theodi/odi_content_models'
end

gem 'erubis'
gem 'exception_notification', '2.6.1', require: false
gem 'formtastic', git: 'https://github.com/justinfrench/formtastic.git', branch: '2.1-stable'
gem 'formtastic-bootstrap', git: 'https://github.com/cgunther/formtastic-bootstrap.git', branch: 'bootstrap-2'

gem 'gds-api-adapters', :github => 'theodi/gds-api-adapters'

gem "nested_form", git: 'https://github.com/alphagov/nested_form.git', branch: 'add-wrapper-class'
gem 'tagmanager-rails'

if ENV['ODIDOWN_DEV']
  gem 'odidown', path: '../odidown'
else
  gem 'odidown', github: 'theodi/odidown'
end

gem 'odlifier', github: 'theodi/odlifier'

gem 'has_scope', '0.5.1'
gem 'inherited_resources', '1.4'
gem 'kaminari', '0.13.0'
gem 'lograge', '0.2.0'
gem 'mongo', '1.7.1'
gem "mongoid_rails_migrations", "1.0.0"
gem 'null_logger'
gem 'plek', '1.4.0'
gem 'rails', '~> 3.2.16'

gem 'redis', '3.0.3', require: false # Only used in some importers
gem 'mlanett-redis-lock', '0.2.2' # Only used in some importers
gem 'rest-client', require: false # Only used in some importers
gem 'retriable', require: false # Only used in some importers
gem 'reverse_markdown', '~> 0.3.0', require: false # Only used in some importers

gem 'statsd-ruby', '1.0.0', require: false
gem 'whenever', require: false

gem 'jquery-rails', '2.0.2'
gem 'less-rails-bootstrap', '~> 2.0.0'
gem 'thin'
gem 'foreman', '< 0.65.0'
gem 'bootstrap-datepicker-rails'
gem 'country-select', :github => 'ninkibah/country-select'
gem 'epic-editor-rails', :github => 'zethussuen/epic-editor-rails'
gem 'fog'
gem 'airbrake'
gem 'mongoid-tree'

group :assets do
  gem "therubyracer", "~> 0.12.0"
  gem 'uglifier'
end

group :development do
  gem 'quiet_assets'
end

group :test do
  gem 'turn', '0.9.6'
  gem 'minitest', '3.3.0'
  gem 'shoulda'
  gem 'database_cleaner'

  gem 'capybara', '1.1.4'
  gem 'poltergeist'
  gem 'launchy'

  gem 'webmock', '~> 1.8.7'
  gem 'mocha', '0.13.3', :require => false
  gem 'factory_girl_rails'
  gem 'faker', '1.1.2'

  gem "timecop"

  gem 'simplecov', '~> 0.6.4', :require => false
  gem 'simplecov-rcov', '~> 0.2.3', :require => false
  gem 'ci_reporter', "~> 1.0"
end
