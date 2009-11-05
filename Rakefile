#!/usr/bin/env ruby

require 'rake'

namespace :juicer do
  desc "Install juicer"
  task :install do
    sh "gem install juicer"
    sh "juicer install yui_compressor" 
    sh "juicer install jslint"
  end
end

namespace :blueprint do
  desc "Update Blueprint CSS framework by downloading the latest version"
  task :update do
    sh "rm -rf stylesheets/blueprint"
    sh "git clone http://github.com/joshuaclayton/blueprint-css.git" 
    sh "cp -R blueprint-css/blueprint stylesheets"
    sh "rm -rf blueprint-css"
  end
end
