[![Gem Version](https://badge.fury.io/rb/omniauth-smartthings.svg)](https://badge.fury.io/rb/omniauth-smartthings)

# Omniauth::SmartThings - SmartThings strategy for OmniAuth 1.x

An OmniAuth strategy for SmartThings OAuth2 integration.

In order to get OAuth client ID/secret, create a SmartThings app on their developer portal.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'omniauth-smartthings'
```

And then execute:

    $ bundle

## Usage

Once you have credentials from SmartThings, you could add the middleware to a Rails app in `config/initializers/omniauth.rb`:

```ruby
Rails.application.config.middleware.use OmniAuth::Builder do
  provider :smartthings, ENV["SMARTTHINGS_CLIENT_ID"], ENV["SMARTTHINGS_CLIENT_SECRET"]
end
```

## Development

After checking out the repo, run `bin/setup` to install dependencies.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/jodyalbritton/omniauth-smartthings.


## License

The gem is available as open source under the terms of the [Apache 2.0 License](http://opensource.org/licenses/Apache-2.0).
