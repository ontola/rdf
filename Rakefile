#!/usr/bin/env ruby
$:.unshift(File.expand_path(File.join(File.dirname(__FILE__), 'lib')))
require 'rubygems'
begin
  require 'rakefile' # http://github.com/bendiken/rakefile
rescue LoadError => e
end
require 'rdf'

desc "Generate etc/doap.nt from etc/doap.ttl."
task :doap do
  sh "rapper -i turtle -o ntriples etc/doap.ttl | sort > etc/doap.nt"
end
