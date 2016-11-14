require 'html-proofer'

task :default do
  sh "bundle exec jekyll build"
  opts = { :check_html => true,
    :url_ignore => [/linkedin.com/], # LinkedIn refuses to serve data to Travis
  }
  HTMLProofer.check_directory('./_site', opts).run
end
