require 'rubygems'
require 'rake'


#############################################################################
#
# Helper functions
#
#############################################################################

def optimizePNG
  # Optimize them all!
  sh 'optipng -o7 ./src/*.png'
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
end

desc 'Publish site to server'
task :publish do
  sh './publish.sh'
end

