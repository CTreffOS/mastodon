custom
===========

## themes
Two themes were added. For both the main color is orange. There is one dark and one light theme.

## install
copy the files from the *custom* directory of this repository to the *live* directory

except the locales, there the lines must be modified.

### Pre-compiling updated assets:
```sh
cd ~/live
RAILS_ENV=production bundle exec rails assets:precompile
```
### Restarting Mastodon services:
```sh
systemctl restart mastodon-sidekiq.service mastodon-streaming.service mastodon-web.service
```
