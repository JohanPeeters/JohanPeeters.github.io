source 'https://rubygems.org'

require 'json'
require 'open-uri'
version_string = open('https://pages.github.com/versions.json'){|json| json.read}
versions = JSON.parse(version_string)
ruby ">= #{versions['ruby']}"
gem 'github-pages', '>= 214', ">= #{versions['github-pages']}"
gem 'nokogiri', '>= 1.12.5', ">= #{versions['nokogiri']}"
gem 'jekyll', '>= 3.9.0', ">= #{versions['jekyll']}"
gem 'jekyll-sitemap', '>= 1.4.0', ">= #{versions['jekyll-sitemap']}"
gem 'font-awesome-sass', '>= 5.4.1'

group :test do
  gem 'rake', '>= 12.3.3'
  gem 'html-proofer', '>= 3.16.0'
end
