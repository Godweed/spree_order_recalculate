SpreeCartUpdate
===============

As spree doesn't update line items price when products price changes, this extension make it. 

Tested with spree 3.0.2.beta.

Installation
------------

Add spree_cart_update to your Gemfile:

```ruby
gem 'spree_cart_update'
```

Bundle your dependencies and run the installation generator:

```shell
bundle
bundle exec rails g spree_cart_update:install
```

Testing
-------

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_cart_update/factories'
```

Copyright (c) 2015 Vladislav Zaets, released under the New BSD License
