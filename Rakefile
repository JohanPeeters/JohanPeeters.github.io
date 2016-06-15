require 'html-proofer'

task :default do
  sh "bundle exec jekyll build"
  opts = { :check_html => true,
    :typhoeus => {
      :headers => { "User-Agent" => "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/42.0.2311.135 Safari/537.36 Edge/12.246" }
    }, # pretend to be a browser lest LinkedIn blocks 'suspicious' request
  }
  HTMLProofer.check_directory('./_site', opts).run
end
