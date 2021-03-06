# Rails Startup template

This is a template I use for my new Ruby on Rails 4 applications. **Pull requests are welcome.**

Also check out [Startup Readings](https://github.com/dennybritz/startupreadings).

## How to Use

```bash
rails new [app_name] --skip-test-unit -m https://raw.github.com/FTW-Development/rails_startup_template/master/template.rb
```

Optionally, you might want to throw in `-d mysql` if using mysql, or `--skip-active-record` if mongodb


## What it does

1. Adds the following gems:
  - [analytics-ruby](https://github.com/segmentio/analytics-ruby): I use [segment.io](https://segment.io/) as an anaytics provider. Segment.io is easy to integrate, asynchronous, and forwards data to other providers like Mixpanel and Kissmetrics.
  - [bourbon](http://bourbon.io/): Bourbon provides useful SASS mixins for cross-browser compatibility.
  - [CanCan](https://github.com/ryanb/cancan): CanCan is an authorization library for Ruby on Rails which restricts what resources a given user is allowed to access.
  - [haml-rails](http://haml.info): HAML is a beautiful templating language. I prefer it over ERB. 
  - [simple_form](https://github.com/plataformatec/simple_form): SimpleForm makes it easy to build complex form using simple markup.
  - [rspec-rails](https://github.com/rspec/rspec-rails): Rspec is a testing tool for test-driven and behavior-driven development. It makes writing specs more enjoyable.
  - [guard-rspec](https://github.com/guard/guard-rspec): Guard for automatically launching your specs when files are modified.
  - (test environment) [capybara](https://github.com/jnicklas/capybara): I use Capybara to write integration tests and simulate user behavior.
  - (test environment) [factory_girl_rails](https://github.com/thoughtbot/factory_girl): FactoryGirl provdes a flexible alternative to Rails fixtures. 

2. Sets up [foreman](https://github.com/ddollar/foreman) to deal with environment variables and background services. Instead of using `rails s` you should use `foreman s`. Add your own environment variables in the `.env` file.

4. Optionally installs [Twitter bootstrap](http://getbootstrap.com/).

5. Optionally installs [Font Awesome](http://fortawesome.github.io/Font-Awesome/).

6. Initializes a new git repository with an initial commit.

7. Optionally create a github repository.

