task :default do
  sh "rspec spec"
end

task :all do
  sh "AR=2.3.12 bundle && bundle exec rake"
  sh "AR=3.0.8 bundle && bundle exec rake"
  sh "AR=3.1.0.rc4 bundle && bundle exec rake"
end

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = 'translated_attributes'
    gem.summary = "ActiveRecord/Rails simple translatable attributes"
    gem.email = "michael@grosser.it"
    gem.homepage = "http://github.com/grosser/#{gem.name}"
    gem.authors = ["Michael Grosser"]
    gem.add_dependency ['activerecord']
  end

  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler, or one of its dependencies, is not available. Install it with: sudo gem install technicalpickles-jeweler -s http://gems.github.com"
end
