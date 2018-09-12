hemphill
========

[![Build Status][status-image]][travis]

All my control repo does is hold configuration hieradata and point to
this GitHub repo.

    $ git clone https://github.com/daaang/hemphill
    $ cd hemphill
    $ bundle install

To run all tests:

    $ bundle exec rake spec
    $ bundle exec rake rubocop
    $ bundle exec rake syntax lint
    $ bundle exec rake metadata_lint

To test a single file, you need to do so between `rake spec_prep` and
`rake spec_clean`:

    $ bundle exec rake spec_prep
    $ bundle exec rspec [spec/specific_file.spec.rb]
    $ bundle exec rspec [spec/any_other_file.spec.rb]
    $ bundle exec rspec [spec/maybe_the_same_file_a_few_times.spec.rb]
    $ bundle exec rspec [spec/maybe_the_same_file_a_few_times.spec.rb]
    $ bundle exec rspec [spec/maybe_the_same_file_a_few_times.spec.rb]
    $ bundle exec rake spec_clean

[travis]:       https://travis-ci.org/daaang/hemphill
[status-image]: https://travis-ci.org/daaang/hemphill.svg?branch=master
