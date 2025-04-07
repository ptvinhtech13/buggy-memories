## How to run for local development?
### Install Ruby 

 ```
 scoop install ruby
 scoop uninstall ruby
 scoop install msys2
 ridk install --> Select 2,3
 gem install ridk
 gem install wdm
 gem update --system
 gem install bundler
 bundle exec jekyll serve --config _config.yml,_config_dev.yml --livereload
 bundle exec jekyll clean
 bundle exec jekyll build
 ```
