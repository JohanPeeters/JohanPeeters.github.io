source 'https://rubygems.org'

require 'json'
require 'open-uri'
version_string = URI.parse('https://pages.github.com/versions.json').to_s
versions = JSON.parse(version_string)
ruby ">= #{versions['ruby']}"
gem 'github-pages', ">= #{versions['github-pages']}"
gem 'nokogiri', ">= #{versions['nokogiri']}"
gem 'jekyll', ">= #{versions['jekyll']}"
gem 'jekyll-sitemap', ">= #{versions['jekyll-sitemap']}"
gem 'font-awesome-sass', '>= 5.4.1'

group :test do
  gem 'rake', '>= 12.3.3'
  gem 'html-proofer', '>= 3.10.0'
end
