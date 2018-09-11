hemphill
========

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

To test a single file:

    $ bundle exec rspec [spec/specific_file.spec.rb]
