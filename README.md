# WELITE Application

This repository contains the source code for the **WELITE** web application.

The project is distributed as a single archive `Script.zip` which, once extracted, provides a PHP-based social networking platform derived from the [Sngine](https://sngine.com/) script. The archive also bundles its PHP dependencies (via `composer`) and JavaScript modules (via `npm`).

## Extracting the Script

To work with the application code you must unzip the `Script.zip` file:

```bash
unzip Script.zip -d src
```

The extracted `src` directory will include all PHP files, assets and vendor libraries required by the system.

## Running Locally

1. Ensure PHP (>=7.4) and a web server such as Apache or Nginx are installed.
2. Create a MySQL database and update the configuration values in `includes/config-example.php` (or copy it to `config.php` and modify as needed).
3. Install composer dependencies if you need to rebuild the vendor directory:

```bash
composer install
```

4. Serve the `src` directory via your web server and point your browser to the configured URL.

## Development Notes

- Node dependencies are listed in `package.json`. If you wish to rebuild assets run:

```bash
npm install
```

- The GitHub Actions workflow under `.github/workflows/aws.yml` demonstrates how a Docker image could be built and deployed to Amazon ECS.

## License

This repository does not contain a license file. Please ensure you have permission to use the included Sngine-based script.
