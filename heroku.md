# Heroku Snippets

### Reset a db to rerun migrations and seeds
- `heroku pg:reset DATABASE -a bullseye-dev` (verify that the DATABASE matches the one in the config vars)
- `heroku run rake db:migrate -a bullseye-dev`
- `heroku run rake db:seed -a bullseye-dev`

## From Penney's Gist

Heroku console:<br>
<code>heroku run console --remote dev</code>

Gmail hack:<br>
<code>marybethburch+whatever@gmail.com</code>marybethburch

Heroku postgres issues:<br>
<code>heroku run rake db:migrate -r <remotename></code>
