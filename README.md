# Heroku buildpack for the official Heroku Toolbelt

The buildpack installs Heroku Toolbelt and adds it to `PATH`. Nice tool if you
need to perform some plumbing.


## Usage

As all other custom buildpacks it might be added to your app with:

    heroku buildpacks:add https://github.com/soulim/heroku-buildpack-toolbelt.git

Next time you deploy the app, the buildpack will be used. If deploy has been
successful, `heroku` command is available for you to run.

## Known issues

Because of Heroku CLI internal design, it updates itself and installed plugins
every time you run `heroku` command. I hope it'll be fixed soon. The issue is 
[reported already][1].

## Copyright information

(c) 2015, Alexander Sulim, <http://sul.im>

[1]: https://github.com/heroku/heroku-cli/issues/129
