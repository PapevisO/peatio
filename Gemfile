# encoding: UTF-8
# frozen_string_literal: true

source 'https://rubygems.org'

ruby File.read('.ruby-version')

gem 'ransack', '~> 2.3.2'
gem 'rails', '~> 5.2.4.5'
gem 'puma', '~> 5.0'
gem 'redis', '~> 4.1.2', require: ['redis', 'redis/connection/hiredis']
gem 'hiredis', '~> 0.6.0'
gem 'figaro', '~> 1.1.1'
gem 'hashie', '~> 3.6.0'
gem 'aasm', '~> 5.0.8'
gem 'bunny', '~> 2.14.1'
gem 'cancancan', '~> 3.1.0'
gem 'enumerize', '~> 2.2.2'
gem 'kaminari', '~> 1.2.1'
gem 'rbtree', '~> 0.4.2'
gem 'grape', '~> 1.3.1'
gem 'grape-entity', '~> 0.7.1'
gem 'grape-swagger', '~> 0.30.1'
gem 'grape-swagger-ui', '~> 2.2.8'
gem 'grape-swagger-entity', '~> 0.2.5'
gem 'grape_logging', '~> 1.8.0'
gem 'rack-attack', '~> 5.4.2'
gem 'faraday'
gem 'faraday_middleware'
gem 'faye', '~> 1.4'
gem 'eventmachine', '~> 1.2'
gem 'em-synchrony', '~> 1.0'

# We use 2.3.0.dev for bitzlato client
# Fill free to update to rubygem version when it will be released
gem 'jwt', github: 'jwt/ruby-jwt'

gem 'email_validator', '~> 1.6.0'
gem 'validate_url', '~> 1.0.4'
gem 'god', '~> 0.13.7', require: false
gem 'arel-is-blank', '~> 1.0.0'
gem "sentry-ruby"
gem "sentry-rails"
gem 'memoist', '~> 0.16.0'
gem 'method-not-implemented', '~> 1.0.1'
gem 'validates_lengths_from_database', '~> 0.7.0'
gem 'jwt-multisig', '~> 1.0.0'
gem 'cash-addr', '~> 0.2.0', require: 'cash_addr'
gem 'digest-sha3', '~> 1.1.0'
gem 'scout_apm', '~> 2.4', require: false
gem 'peatio', github: 'bitzlato/peatio-core'
gem 'rack-cors', '~> 1.0.6', require: false
gem 'jwt-rack', '~> 0.1.0', require: false
gem 'env-tweaks', '~> 1.0.0'
gem 'vault', '~> 0.12', require: false
gem 'vault-rails', github: 'finfex/vault-rails'
gem 'bootsnap', '>= 1.1.0', require: false
gem 'net-http-persistent', '~> 3.0.1'
gem 'influxdb', '~> 0.7.0'
gem 'safe_yaml', '~> 1.0.5', require: 'safe_yaml/load'
gem 'dotenv'

# Security versions of deep dependencies
gem "addressable", ">= 2.8.0"
gem "rexml", ">= 3.2.5"

group :development, :test do
  gem 'irb'
  gem 'bump',         '~> 0.7'
  gem 'faker',        '~> 1.8'
  gem 'pry-byebug',   '~> 3.7'
  gem 'bullet',       '~> 5.9'
  gem 'grape_on_rails_routes', '~> 0.3.2'
end

group :development do
  gem 'foreman'
  gem 'annotate',   '~> 3.1.0'
  gem 'ruby-prof',  '~> 0.17.0', require: false
  gem 'listen',     '>= 3.0.5', '< 3.2'

  gem 'rspec'
  gem 'guard'
  gem 'guard-rspec', github: 'caspark/guard-rspec' # Use from github to remove rspec < 4.0 dependencies
end

group :test do
  gem 'rspec-rails', '~> 3.8', '>= 3.8.2'
  gem 'rspec-retry',         '~> 0.6'
  gem 'webmock',             '~> 3.5'
  gem 'database_cleaner',    '~> 1.7'
  gem 'mocha',               '~> 1.8', require: false
  gem 'factory_bot_rails', '~> 5.0', '>= 5.0.2'
  gem 'timecop',             '~> 0.9'
  gem 'rubocop-rspec',       '~> 1.32', require: false
end

# Load gems from Gemfile.plugin.
Dir.glob File.expand_path('../Gemfile.plugin', __FILE__) do |file|
  eval_gemfile file
end

gem "pg", "~> 1.2"

gem "http_accept_language", "~> 2.1"

gem "semver2", "~> 3.4"

group :deploy do
  gem 'capistrano-dotenv'
  gem 'capistrano-dotenv-tasks'
  gem 'capistrano3-puma', github: 'seuros/capistrano-puma'
  gem 'capistrano', require: false
  gem 'capistrano-rbenv', require: false
  gem 'capistrano-rails', require: false
  gem 'capistrano-bundler', require: false
  gem 'capistrano-shell', require: false
  gem 'capistrano-db-tasks', require: false
  gem 'capistrano-rails-console', require: false
  gem 'capistrano-tasks', github: 'brandymint/capistrano-tasks', require: false
  gem 'capistrano-systemd-multiservice', github: 'groovenauts/capistrano-systemd-multiservice', require: false
  # gem 'capistrano-master-key', require: false, github: 'virgoproz/capistrano-master-key'
  gem 'capistrano-git-with-submodules'
  gem 'capistrano-sentry', require: false
  gem 'slackistrano', require: false
end

gem "sd_notify", "~> 0.1.1"
