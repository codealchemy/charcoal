require 'bundler/setup'
require 'bundler/gem_tasks'
require 'wwtd/tasks'
require 'bump/tasks'
require 'rake/testtask'

Rake::TestTask.new(:test) do |test|
  test.libs << 'lib' << 'test'
  test.pattern = 'test/**/*_test.rb'
  test.verbose = true
end

task :default => 'wwtd:local'

require 'yard'
YARD::Rake::YardocTask.new
