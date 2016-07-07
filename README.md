# Heroku Buildpack Gulp

A simple buildpack, designed to run with the [multi buildpack](https://github.com/ddollar/heroku-buildpack-multi),
and runs `gulp`.

## Usage

1. Set your buildpack to the [multi buildpack](https://github.com/ddollar/heroku-buildpack-multi):

   ```bash
   $ heroku config:set BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi
   ```

2. Configure your `.buildpacks` file:

   ```
   https://github.com/heroku/heroku-buildpack-nodejs
   https://github.com/umurkontaci/heroku-buildpack-gulp
   ```

3. Ensure that npm installs bower:

   ```json
   {
     "dependencies": {
       "gulp": "latest"
     }
   }
   ```
