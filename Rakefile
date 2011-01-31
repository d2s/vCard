task :default => :generate

desc 'Generate vCard site'
task :generate do
  optimizePNG
  sh 'cp ./src/*.vcf ./build/'
  sh 'python ./scripts/builder.py'
  #sh './scripts/publish.sh'
end

def optimizePNG
  # Optimize them all!
  sh 'optipng -o7 ./src/*.png'
end