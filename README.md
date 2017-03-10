REC Master
=========

1. bundle install
2. copy config/*.yml.sample to .yml
3. bin/rake recognize:init

## Running server
+ Create hostname to l.recognizeapp.com
+ Run server on port 500000
    
    ````
    bin/rails s -p50000
    bin/rails_ssl(SSL - need self signed cert and key in ~/.ssl)
    ````
    
## Running tests

    RAILS_ENV=test bin/rake recognize:init # first time only
    bin/rspec spec

##Dependencies
+ Qt(for capybara-webkit)
+ libv8
+ Mysql(v5.6.x)

## Mailcatcher(for local mail delivery)

    gem install mailcatcher
