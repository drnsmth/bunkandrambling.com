
task :default => [:generate]

task :refresh do 
  sh "git pull git@src.bunkandrambling.com:bunkandrambling.git"
end

task :clean do
  sh "rm -rf _site"
end

task :generate do
  sh "jekyll"
  sh "mv _site/atom.html _site/atom.xml"
end

task :publish => [:clean, :refresh, :generate] do 
  cp "_site/* /var/www/" 
  sh "chown -R wwwdata:wwwdata /var/www/*"
end
