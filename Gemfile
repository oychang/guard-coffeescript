source 'https://rubygems.org'

gemspec

gem 'rake'

platform :ruby_18 do
  gem 'json'
end

# The JS runtime is needed because ExecJS searches one when the module is loaded.
# This breaks travis builds even when the compiler is stubbed.
platform :jruby do
  gem 'therubyrhino'
end

unless ENV['TRAVIS']
  gem 'redcarpet'
  gem 'yard'
end
