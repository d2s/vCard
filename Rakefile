require 'rubygems'
require 'rake'
require 'manifesto'


#############################################################################
#
# Helper functions
#
#############################################################################

def optimizePNG
  # Optimize them all!
  sh 'optipng -o7 ./src/*.png'
end

def cachebuilder
  # Creates .manifest for files in build directory
  Manifesto.cache :directory => './build'
end



#############################################################################
#
# Standard tasks
#
#############################################################################

task :default => [:generate, :publish]

desc 'Generate vCard site'
task :generate do
  optimizePNG
  sh 'cp ./src/*.vcf ./build/'
  sh 'python ./scripts/builder.py'
  #cachebuilder
end

desc 'Publish site to server'
task :publish do
  sh './publish.sh'
end

