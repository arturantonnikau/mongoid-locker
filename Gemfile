source 'https://rubygems.org'
gemspec

case ENV['MONGOID_VERSION']
when /^7/
  gem 'mongoid', '~> 7.0'
when /^6/
  gem 'mongoid', '~> 6.4'
when /^5/
  gem 'mongoid', '~> 5.4'
else
  gem 'mongoid', '>= 5.0'
end

gem 'rake'

group :development do
  gem 'guard-rspec'
end

group :development, :test do
  gem 'pry-byebug', platforms: :mri

  gem 'mongoid-danger', '~> 0.1.1'
  gem 'rspec', '~> 3.8'
  gem 'rubocop'
  gem 'rubocop-rspec'
  gem 'simplecov', require: false
end
