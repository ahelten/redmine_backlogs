source 'https://rubygems.org'

chiliproject_file = File.dirname(__FILE__) + "/lib/chili_project.rb"
chiliproject = File.file?(chiliproject_file)

deps = Hash.new
@dependencies.map{|dep| deps[dep.name] = dep }
rails3 = Gem::Dependency.new('rails', '~>3.0')
RAILS_VERSION_IS_3 = rails3 =~ deps['rails']

gem "holidays", "~>1.0.3"
gem "icalendar", "1.3.0"
gem "nokogiri", "< 1.6.0"
gem "open-uri-cached","0.0.5"
gem "prawn","0.7.1"
# Disable version specification, it conflicts with other plugins
#gem 'json',"1.8.3"
gem 'json'
gem "system_timer" if RUBY_VERSION =~ /^1\.8\./ && RUBY_PLATFORM =~ /darwin|linux/

