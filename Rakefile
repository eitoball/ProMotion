$:.unshift("/Library/RubyMotion/lib")
require 'motion/project'
require 'bundler/gem_tasks'
Bundler.setup
Bundler.require

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'ProMotionTest'
  app.version = "0.0.1"

  # Devices
  app.deployment_target = "4.3"
  app.device_family = [:iphone, :ipad]

  # Preload screens
  app.files = Dir.glob(File.join(app.project_dir, 'lib/**/*.rb')) | app.files
end
