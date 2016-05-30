require 'html-proofer'

task :default do
  sh "bundle exec jekyll build"
  opts = {}
  HTMLProofer.check_directory('./_site', opts).run
end
