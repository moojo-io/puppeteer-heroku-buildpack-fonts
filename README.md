# puppeteer-heroku-buildback-fonts

Heroku buildpack adding fonts needed to render moojo documents.

Based on https://github.com/gnuletik/puppeteer-heroku-buildpack-fonts

## Usage

```sh-session
# clear cache and current buildpacks
heroku builds:cache:purge
heroku buildpacks:clear

# puppeteer
heroku buildpacks:add -i 1 jontewks/puppeteer

# fonts
heroku buildpacks:add -i 2 https://github.com/moojo-io/puppeteer-heroku-buildpack-fonts

# other buildpack
heroku buildpacks:add -i 3 heroku/nodejs
```
