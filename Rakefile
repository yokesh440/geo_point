# encoding: utf-8

require 'rubygems'
require 'bundler'
begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end
require 'rake'

require 'jeweler'
Jeweler::Tasks.new do |gem|
  # gem is a Gem::Specification... see http://docs.rubygems.org/read/chapter/20 for more options
  gem.name = "geo_point"
  gem.homepage = "http://github.com/kristianmandrup/geo_point"
  gem.license = "MIT"
  gem.summary = %Q{A GeoPoint encapsulates latitude, longitude and various geo calculations relative to itself}
  gem.description = %Q{Allows for easy parsing of Strings, Hashes and Arrays into a GeoPoint with lat/long}
  gem.email = "kmandrup@gmail.com"
  gem.authors = ["Kristian Mandrup"]
  # dependencies defined in Gemfile
end
Jeweler::RubygemsDotOrgTasks.new

require 'rspec/core'
require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec) do |spec|
  spec.pattern = FileList['spec/**/*_spec.rb']
end

task :default => :spec

