
task :default => [:generate]

task :refresh do 
  sh "git pull git@src.bunkandrambling.com:bunkandrambling.git"
end

task :clean do
  sh "rm -rf _site"
end

task :generate do
  sh "jekyll"
end

task :publish => [:clean, :generate] do 
  sh "cp -r _site/* /var/www/" 
  sh "chown -R www-data:www-data /var/www/*"
end
