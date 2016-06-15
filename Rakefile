require 'html-proofer'

task :default do
  sh "bundle exec jekyll build"
  opts = { :check_html => true,
    :typhoeus => {
      :headers => { "User-Agent" => "Mozilla/5.0 (compatible; My New User-Agent)" }
    }, # pretend to be a browser lest LinkedIn blocks 'suspicious' request
  }
  HTMLProofer.check_directory('./_site', opts).run
end
