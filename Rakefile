require 'rubygems'
require 'bundler'
Bundler.setup

require 'rdiscount'

task :default do
  markdown = RDiscount.new(File.read('resume.markdown'))
  puts "Writing index.html"
  File.open('index.html', 'w') do |f|
    f << markdown.to_html
  end
end