# FAIR Testing

An environment for testing the [FAIR Connect plugin](https://github.com/fairpm/fair-plugin) for WordPress.

## Setup

1. Install dependencies:

       composer install

2. Start the local development environment:

       npx @wordpress/env start -- --xdebug

3. Visit http://localhost:8888 and login with `admin` / `password`.

4. Install and activate the [FAIR Connect plugin](https://github.com/fairpm/fair-plugin) by either installing it via WordPress admin or cloning the repository under `wp-content/plugins`. Note: it can't be added via Composer until https://github.com/fairpm/fair-plugin/issues/505 is fixed.

5. Update the `Version: ...` header in any of the plugins to a lower version and test the "FAIR Connect" plugin upgrade process.