source 'https://rubygems.org'

group :development, :test do
  gem 'rake'
  gem 'rspec-puppet'
  gem 'metadata-json-lint'
  gem 'puppetlabs_spec_helper'
  gem 'puppet-lint', :git => 'https://github.com/rodjek/puppet-lint.git'
  gem 'puppet-lint-absolute_classname-check'
  gem 'puppet-lint-alias-check'
  gem 'puppet-lint-empty_string-check'
  gem 'puppet-lint-file_ensure-check'
  gem 'puppet-lint-file_source_rights-check'
  gem 'puppet-lint-fileserver-check'
  gem 'puppet-lint-leading_zero-check'
  gem 'puppet-lint-spaceship_operator_without_tag-check'
  gem 'puppet-lint-trailing_comma-check'
  gem 'puppet-lint-undef_in_function-check'
  gem 'puppet-lint-unquoted_string-check'
  gem 'puppet-lint-variable_contains_upcase'
end

if puppetversion = ENV['PUPPET_GEM_VERSION']
  gem 'puppet', puppetversion, :require => false
else
  gem 'puppet', :require => false
end

# rspec must be v2 for ruby 1.8.7
if RUBY_VERSION >= '1.8.7' and RUBY_VERSION < '1.9'
  gem 'rspec', '~> 2.0'
end
