# Dot Ledger [![Build Status](https://api.travis-ci.org/dotledger/dotledger.svg?branch=master)](https://travis-ci.org/dotledger/dotledger) [![Code Climate](https://codeclimate.com/github/dotledger/dotledger/badges/gpa.svg)](https://codeclimate.com/github/dotledger/dotledger)

**[Dot Ledger](http://www.dotledger.com/)** is a Free and Open Source personal finance management tool.

The aim of this project is to create a stable, FOSS alternative to [Xero Personal](https://www.xero.com/personal/)
which was [shut down](http://blog.xero.com/2013/08/winding-down-xero-personal-in-november-2014/) in November 2014.

## Setup

Dot Ledger requires:

- [PostgreSQL](https://www.postgresql.org/) (Tested with 9.6)
- [Ruby](https://www.ruby-lang.org/) (Tested with 2.3)
- [RubyGems](https://rubygems.org/)
- [Ruby on Rails](http://rubyonrails.org/)
- [Bundler](https://bundler.io/)
- [Git](https://git-scm.com/)

The basic setup steps are:

- `git clone https://github.com/dotledger/dotledger.git`
- `cd dotledger`
- `cp config/database.yml.example config/database.yml`

You'll have to modify the postgres username and password in `config/database.yml`.

- `bundle install`
- `bundle exec rake db:setup`
- `bundle exec rails server`

## Tests

### Run all tests

```
bundle exec rake spec spec:javascript
```

### Run ruby tests ([RSpec](http://rspec.info/))

```
bundle exec rake spec
```

### Run javascript tests ([Jasmine](http://jasmine.github.io/))

```
bundle exec rake spec:javascript
```

## Screenshots

See [the screenshots section](http://www.dotledger.com/#screenshots) of the [Dot Ledger website](http://www.dotledger.com/).

## License

Copyright 2013 - 2018, Kale Worsley, BitBot Limited.

Dot Ledger is made available under the Apache License, Version 2.0. See [LICENSE](LICENSE) for details.
