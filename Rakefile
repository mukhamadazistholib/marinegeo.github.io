#!/usr/bin/env ruby

require "rake/testtask"
require "html-proofer"

test = Rake::TestTask.new do
  options = {
    :check_external_hash => true,
    :check_html => true,
    :check_opengraph => true,
    :http_status_ignore => [1..403, 405..999],
    :typhoteus => {
      :ssl_verifypeer => false,
      :ssl_verifyhost => 0
    },
    :cache => {
      :timeframe => '6w'
    },
    :assume_extension => true,
    :external_only => false,
  }
  begin
    HTMLProofer.check_directory("./_site", options).run
  rescue => msg
    puts "#{msg}"
  end
end

task :default => :test
