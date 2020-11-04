source 'https://rubygems.org'

require 'json'
require 'open-uri'
version_string = URI.parse('https://pages.github.com/versions.json').read
versions = JSON.parse(version_string)
ruby ">= #{versions['ruby']}"
gem 'github-pages', '>= 207', ">= #{versions['github-pages']}"
gem 'nokogiri', '>= 1.10.8', ">= #{versions['nokogiri']}"
gem 'jekyll', '>= 3.9.0', ">= #{versions['jekyll']}"
gem 'jekyll-sitemap', '>= 1.2.0'
gem 'font-awesome-sass', '>= 5.4.1'

group :test do
  gem 'rake', '>= 12.3.3'
  gem 'html-proofer', '>= 3.10.0'
end
