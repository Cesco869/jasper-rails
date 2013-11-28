require "bundler/gem_tasks"

namespace :jasper do

  desc 'run mavern to download jars'
  task :install do
    `rm lib/java/*.jar`
    Kernel.puts `mvn dependency:copy-dependencies -DoutputDirectory=lib/java`
  end
end
