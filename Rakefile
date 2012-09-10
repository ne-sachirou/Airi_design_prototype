# encoding = utf-8

desc 'compile SCSS.'
task :scss do
  style_dir = 'styles'
  Dir["#{style_dir}/*.scss"].each do |filename|
    basename = "#{style_dir}/#{File.basename filename, '.scss'}"
    sh "scss --style compressed #{filename} #{basename}.css"
  end
end
