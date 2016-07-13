# VineDl

A rubygem to auth in and rip a users Vine videos.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'vine_dl'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install vine_dl

## Usage

```ruby
VineDl.login_and_get_videos("VINE_USERNAME", "VINE_PASSWORD")
```

The gem will create a `downloads` directory in the root
of the project folder with the returned video files in it.

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Running tests

Simply run the rake command.

```shell
rake
# or
rake test
```

You can configure `.env` to disable mocks in tests.
This requires valid credentials in ENV.

```shell
VINE_USERNAME=YOUR_REAL_VINE_USERNAME
VINE_PASSWORD=YOUR_REAL_VINE_PASSWORD
NO_MOCKS=false
```

You can tell the tests not to delete the files it downloads.

```shell
VINE_USERNAME=YOUR_REAL_VINE_USERNAME
VINE_PASSWORD=YOUR_REAL_VINE_PASSWORD
NO_MOCKS=false
NO_DELETE_DOWNLOADED_FILES=false
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/dannyvassallo/vine_dl. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
