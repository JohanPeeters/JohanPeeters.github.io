require 'html-proofer'

task :default do
  sh "bundle exec jekyll build"
  opts = { :check_html => true,
    :typhoeus => {
      :headers => { "User-Agent" => "Mozilla/5.0 (Windows; U; Windows NT 6.1; rv:2.2) Gecko/20110201" }
    }, # pretend to be a browser lest LinkedIn blocks 'suspicious' request
  }
  HTMLProofer.check_directory('./_site', opts).run
end
