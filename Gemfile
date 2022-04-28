source 'https://rubygems.org'

gem 'rails', '5.2.7.1'
gem 'rails-ujs' # Rails unobtrusive scripting adapter; this was moved into Rails in 5.1 - it can be removed when we upgrade

gem 'mimemagic', '~> 0.3.4'

gem 'aws-sdk-s3', '~> 1.84' # AWS S3 module, (aws-sdk v3) - Swapped with aws-sdk, as newest version will pull in ALL modules. If other modules needed, require those separately.


gem 'unicorn', '5.4.0' #use unicorn as webserver
gem 'unicorn-rails', '2.2.1' #point `rails s` to unicorn
gem 'unicorn-worker-killer', '0.4.4' #manage unicorn worker procs based on requests/memory use

gem 'mysql2', '~> 0.5.0'

gem 'scout_apm', '4.0.1' # APM for dev/prod environments; config is config/scout_apm.yml
gem 'graphql', '1.11.4' # API query language
gem 'graphql-guard', '2.0.0' # field level auth for graphql

gem 'bcrypt', '3.1.11' #for ActiveModel has_secure_password
gem 'american_date', '1.1.0' #parses american dates like Date.parse('12/24/2014')
gem 'rest-client', '~> 2.1.0'#used by Walrus and TokenClient to POST
gem "nokogiri", '>= 1.10.10' #used to parse XML by Vertex, and Milliman
gem 'twilio-ruby', '~> 5.34.0' #used to send text messages for 2FA and other text messaging requiremments
gem 'rmagick', '2.16.0' #used to do image uploads/cropping

gem 'bluepill', '0.1.3' #bluepill
gem 'gearman-ruby', '3.0.7', require: ['gearman', 'gearman/server'] #gearman
gem 'dalli', '2.7.6' #memcached; if upgrading/removing, see config/initializers/dalli_request_errors.rb
gem 'mechanize', '2.7.6' #used by ach processor and fedbank processor to programatically interact with websites
gem 'oauth', '0.4.7' #used by API to do oauth
gem 'doorkeeper', '5.0.3' # used by APIs to handle oauth2 provider functionality
gem 'doorkeeper-openid_connect', '1.6.3' # implements an openid connect authentication on top of doorkeeper gem
gem 'prawn', '0.13.2' #pdf writing used by tax document generation, employment verification letter etc.
gem 'combine_pdf', '1.0.21' # used to easily split and combine pdfs
gem 'identity_cache', '0.5.1' #caching library
gem 'cityhash', '0.8.1' #for identitycache, On MacOS install with:   CXX=/usr/bin/clang++ gem install cityhash
gem 'riif', '0.9.0' #quickbooks iif generation
gem 'salesforce_bulk', :git => "https://github.com/justworkshr/salesforce_bulk.git"
gem 'icalendar', '2.2.2' #used for ical integration
gem 'react-rails', '~> 1.6.2' #removable after webpack introduced
gem 'jira-ruby', require: ['jira'] #make tickets in JIRA, used by compliance
gem 'rufus-scheduler', '3.6.0 ' #the new crontab
gem 'net-ssh', '5.2.0' #used to communicate with 3rd parties
gem 'net-sftp','2.1.2' # used to talk to 3rd parties
gem 'rotp', '3.0.1' # OTP gem for two factor auth. handles generating secret key and validating one time code based on key
gem 'rqrcode', '0.10.1' # generates qr codes given a string.
gem 'hellosign-ruby-sdk', '3.7.7' #used for i9s and other document signing
gem 'integer-obfuscator', '0.1.0' # used for generating a "tax id" from an id in CIC+ EOY reporting
gem 'pundit', '1.1.0' # Used for internal permissions
gem 'uglifier', '3.0.0' #Ruby wrapper for UglifyJS JavaScript compressor. Used in production assets compression.
gem 'quickbooks-ruby', '0.6.6' #qbo
gem 'xeroizer', '2.20.0' #xero
gem 'stupidedi', '1.3.23' #used for aetna EDI
gem 'plaid', '7.0.0' #plaid
gem 'ruby-pardot', '~> 1.3.0'  # Pardot gem for server integration
gem 'netsuite', '0.8.5' #API wrapper for Netsuite
gem 'fixy', :git => "https://github.com/justworkshr/fixy.git", :tag => 'v0.4.2' # Generate fixed width flat files

gem 'rollbar', '3.1.1' # exception reporting

gem 'capistrano', '3.5.0' #capistrano
gem 'capistrano-bundler', '1.1.4'
gem 'capistrano-rails', '1.1.6'
gem 'capistrano-rvm', '0.1.2'

gem 'faye-websocket', '>= 0.11.0' #used by walrus

gem 'paper_trail' #used to keep versioned history of bank_account and member

gem 'elasticsearch', '7.5.0'
gem 'posix-spawn' #for executing system commands without using fork()! no more out of memory errors

gem 'statsd-instrument', git: "https://github.com/justworkshr/statsd-instrument.git", branch: 'jw-2.9.2'
gem 'rubyzip', ">= 1.3.0", require: 'zip' # Used for reading and writing zip files

gem 'jquery-rails' #jquery bundle for rails - allows those horrible fake POST links and :remote => true - we should remove but cant yet

gem 'sassc-rails' #sass

gem 'capistrano3-unicorn'

gem 'geoip'
gem 'useragent' # Used in Two-factor autentication (2FA) for parsing user agent strings to get browser and device information

# makara gem for read-write from master/replicas
gem 'makara'
gem 'pg'
gem 'browser'

# lograge for formatting ruby logs to put in elasticsearch via logstash
# and make them searchable
gem "lograge"
gem "logstash-event"

# quickbase for interfacing with pfpg

# string-similarity gem implements Levenshtein and Cosine distance
# Used to compare PFPG data to our own to generate fraud alerts
gem 'string-similarity'

gem 'marginalia', '1.9.0' # Annotates SQL queries with controller/action/sidekiq job

# https://github.com/Shopify/bootsnap
gem 'bootsnap', require: false

# https://github.com/lostisland/faraday
gem 'faraday', '<= 1.0'

# https://github.com/krisleech/wisper
# Provides an API to use the Publisher / Subscriber pattern
gem 'wisper', '2.0.0'

# https://github.com/krisleech/wisper-sidekiq
# Enables the use of sidekiq to asynchronously react to events published by Wisper
gem 'wisper-sidekiq', '~> 1.0'

# https://github.com/zendesk/zendesk_api_client_rb
gem "zendesk_api", '~> 1.28'

gem "json", "~> 2.3.1"
gem "mime-types", "~> 3.3.1"

group :development do
  # dev debugging tools
  gem 'web-console', '3.0.0' #debugger
  gem 'letter_opener', '1.4.1'

  # dev performance tools
  gem 'stackprof' # ruby call profiler https://github.com/tmm1/stackprof
  gem 'flamegraph' # https://github.com/SamSaffron/flamegraph
  gem 'graphql-playground'
end

group :development, :test do
  gem "rspec_junit_formatter", "~> 0.4.1"
  gem 'rubocop-checkstyle_formatter', require: false # Rubocop plugin to interface with Jenkins to report linting failures
  gem 'rubocop-performance', require: false # Rubocop plugin to help with known performance metrics
  gem 'rubocop-rspec', '1.35.0', require: false # Rubocop rules for RSpec tests
  gem 'rubocop-thread_safety', require: false # Rubocop plugin to check for patterns that are not thread safe.
  gem 'rubocop', '0.74.0', require: false
  gem "rubocop-rails", require: false # Rubocop plugin to check for rails best practices

  gem 'pry', '0.10.3' # locking to prevent runtime issues
  gem 'pry-rails', '0.3.4' #removable possibly - dupe of byebug
  gem 'pry-byebug', '3.4.0' #debugger that responds to binding.pry and byebug
  gem 'annotate', '~> 2.7.4' #provides annotation at top of files by running annotate
  gem 'timecop', '0.7.0' #allows us to simulate system time in tests

  gem 'rspec-rails', '~> 3.8', '>= 3.8.2'
  gem 'database_cleaner', '1.5.3' #Cleans database between mini test runs
  gem 'rails-controller-testing'
  gem 'meta_request', '>= 0.7.2' # Required in order to use rails panel https://github.com/dejan/rails_panel

  gem 'brakeman' #static analysis tool for security
  gem 'parallel_tests'
  gem 'test-prof' # surface test suite metrics
end

group :test do
  gem 'mocha' #mocking and stubbing
  gem 'simplecov', require: false
  gem 'simplecov-lcov', require: false
  gem "vcr", "~> 6.0"
  gem "webmock", "~> 3.11"

end

group :development, :test, :staging, :sandbox do
  gem 'factory_bot', '~> 4.10.0', require: false # factories for testing and preconfigs
end

gem 'google-api-client', require: 'google/apis/calendar_v3'#Used to add approved PTO requests to the client's google calendar.

gem "einhorn", "~> 0.7.4"
gem "redis", "4.1.2"

# used in the whats new panel
# https://www.contentful.com/developers/docs/references/content-delivery-api/
gem 'contentful', '~> 2.15.3'

# used for GPG encryption/decryption of e-IWO files
# https://github.com/rocketjob/iostreams
gem 'iostreams', '1.0.0.beta7'

gem 'graphiql-rails', group: :development

gem "request_store", "~> 1.4"

# for catching/retrying blocks of code (e.g. third-party api requests)
gem 'retriable', '3.1.2'

# Gem to integrate with Salesforce REST APIs
# https://justworks.atlassian.net/wiki/spaces/Prod/pages/610306139/SalesForce+API+integration
gem 'restforce', '~> 3.1.0'

# Gem to generate XLSX (Excel) files, for COVID PPP Report
gem 'caxlsx_rails', '0.6.2'

# Gem to style excel files
gem 'axlsx_styler', '1.0.0'

gem "phonelib", "~> 0.6.43"

gem "roo", "~> 2.8.0"

gem "tzinfo-data", "1.2020.1"

# Gem to track individual sidekiq job
# https://github.com/utgarda/sidekiq-status
gem 'sidekiq-status', "~> 1.1.4"

gem 'ddtrace', '0.42.0'

gem 'sidekiq-worker-killer', '~> 1.0'

gem 'sendgrid-actionmailer', '3.1.1'
