# Ruby and Rails Snippets

### Log

- `tail -f development.log` and `Rails.logger.info` to see what’s up
- `tail -f log/test.log` for testing help

### General Tips
In application.rb to customize generators:

```ruby
config.generators do |g|
  g.orm            :active_record
  g.template_engine :erb
  g.test_framework :test_unit, fixture: true
end
```

## From Penney's Gist

Use guard for running individual tests:<br>
- <code>bundle exec guard</code>
- grab file paths of failing tests and open them in editor
- when you change and save on any test it will run that one test in guard
