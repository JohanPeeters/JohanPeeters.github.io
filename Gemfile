source 'https://rubygems.org'

require 'json'
require 'open-uri'
version_string = URI.parse('https://pages.github.com/versions.json').read
versions = JSON.parse(version_string)
gem 'github-pages', "#{versions['github-pages']}"
ruby "#{versions['ruby']}"
gem 'font-awesome-sass'

group :test do
  gem 'rake'
  gem 'html-proofer'
end
