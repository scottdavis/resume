require 'rubygems'
require 'bundler'
Bundler.setup

require 'rdiscount'

task :default do
  markdown = RDiscount.new(File.read('resume.markdown'))
  puts "Writing resume.html"
  File.open('resume.html', 'w') do |f|
    f << markdown.to_html
  end
end