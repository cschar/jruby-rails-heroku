# README

test project running jruby on heroku

gemfile uses
 - ruby 2.3 
 - jruby-9.1.12.0
 - rails 4.2.9  (rails 5 seems to not support java postgres adapter currently)



```
heroku create --remote jruby-heroku
heroku addons:create heroku-postgresql

git push jruby-heroku master
heroku run rake db:migrate
```