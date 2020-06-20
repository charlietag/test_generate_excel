# README
* Try rails gem
  * https://github.com/caxlsx/caxlsx_rails

## Packages

* Ruby version
  * 2.7.0

* Rails version
  * 6.0.3.2

## Basic setup
* Gems - useful for dev
  * gem 'pry-rails', :group => :development
  * gem 'bullet', group: 'development'

	```bash
	# basic useful dev packages
	gem 'pry-rails', :group => :development
	gem 'bullet', group: 'development'
	```

* jQuery
  * yarn add jquery
    * test_rails_delayedjob_mailer_simpleform/app/javascript/packs/application.js

      ```bash
      import "jquery/src/jquery"
      ...
      ```

* bootstrap
  * yarn add bootstrap popper.js (don't add popper v2, bootstrap default requires v1.16) , (no need to import popper.js manually, bootstrap will do it automatically)
    * app/javascript/packs/application.js
      * `import "bootstrap/dist/js/bootstrap"`
    * app/assets/stylesheets/application.css
      * `*= require 'bootstrap/dist/css/bootstrap'`

## Rails setup

* generate Book
  * `bin/rails g scaffold Book name:string author:string`


## config - credential

* command
  * `EDITOR=vim bundle exec rails credentials:edit`

    ```
    development:
      db:
        user: user
        pass: pass

    production:
      db:
        user: user
        pass: pass
    ```

## Changes
* Basic config and setup
  * https://github.com/charlietag/test_generate_excel/compare/v0.0.0...master
* Start to test caxlsx_rails
  * https://github.com/charlietag/test_generate_excel/compare/v0.0.1...master

## Final Result

![caxlsx_rails_sample.png](/screenshots/caxlsx_rails_sample.png)
