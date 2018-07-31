# Project Setup Checklist
Here's a Rails/React/Redux setup checklist. It should only serve as a reminder. Pulled from __a/A__ site: `2018/07/30`

* [ ] `rails new`
  * Add `--database=postgresql` if using Postgres.
  * Add `--skip-turbolinks` to skip the turbolinks gem.
* [ ] Update your `Gemfile`.
  * `better_errors`
  * `binding_of_caller`
  * `pry-rails`
  * `annotate`
  * `bcrypt`
  * `jquery-rails` (When using rails 5.1+)
* [ ] `bundle install`
* [ ] When using Rails 5.1+, update your `application.js` manifest to include:
  * `//= require jquery`
  * `//= require jquery_ujs`
* [ ] `git init`
  * Update your `.gitignore`.
    * `node_modules/`
    * `bundle.js`
    * `bundle.js.map`
* [ ] `git remote add` the proper remote.
  * `git push -u` the remote.
* [ ] `npm init --yes` to create a package.json file with the default setup.
* [ ] Create a frontend folder at the root of your project with an entry file inside of it.
* [ ] `npm install --save`
  * `webpack`
  * `webpack-cli`
  * `react`
  * `react-dom`
  * `react-router-dom`
  * `redux`
  * `react-redux`
  * `babel-core`
  * `babel-loader`
  * `babel-preset-react`
  * `babel-preset-env`
  * `lodash` (optional)
* [ ] Create a `webpack.config.js` file.
  * The entry point should be in frontend, e.g. `entry: 'frontend/index.jsx'`.
  * The output path should be `'app/assets/javascripts'`.
  * Configure your `module.loaders` to use Babel transpilation for:
    * JSX
    * ES6
  * Include `devtool: 'source-map'`.
* [ ] `git commit` again (Verify that your `.gitignore` works).
  * `git push` your skeleton.
