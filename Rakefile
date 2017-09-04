require 'fileutils'

task :default => :build
task :build => ['dist/index.html']

directory 'dist'

file 'dist/index.html' => ['www/index.html', 'dist'] do
  cp 'www/index.html', 'dist/index.html'
end

task :clean do
  FileUtils.rm_rf 'dist'
end
