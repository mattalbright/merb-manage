#
# Rakefile      Defines the Gem package specification
#
require "rubygems"
require "rake/gempackagetask"

spec = Gem::Specification.new do |s|
  s.name = "merb-manage"
  s.version = "0.4.2"
  s.author = "Matt Albright"
  s.email = "mattalbright@yahoo.com"
  s.homepage = "http://github.com/mattalbright/merb-manage"
  s.platform = Gem::Platform::RUBY
  s.summary = "Provides easy configuration and management of Merb applications, including multiple servers and different adapters"
  s.files = FileList["{bin,config,resources}/**/*"].to_a
  s.executables << "merb-manage-ctl"
end

# Setup the package task
Rake::GemPackageTask.new(spec) do |pkg|
  pkg.need_tar = true
end
