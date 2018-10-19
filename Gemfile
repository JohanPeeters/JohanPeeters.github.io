source 'https://rubygems.org'

require 'json'
require 'open-uri'
version_string = URI.parse('https://pages.github.com/versions.json').read
versions = JSON.parse(version_string)
ruby ">= #{versions['ruby']}"
gem 'github-pages', ">= #{versions['github-pages']}"
gem 'nokogiri', ">= #{versions['nokogiri']}"
gem 'jekyll', ">= #{versions['jekyll']}"
gem 'font-awesome-sass'

group :test do
  gem 'rake'
  gem 'html-proofer'
end
