# PHPStan - PHP Static Analysis Tool

[![Build Status](https://travis-ci.com/phpstan/phpstan-src.svg?branch=master)](https://travis-ci.com/phpstan/phpstan-src)
[![Build](https://github.com/phpstan/phpstan-src/workflows/Build/badge.svg)](https://github.com/phpstan/phpstan-src/actions)
[![PHPStan Enabled](https://img.shields.io/badge/PHPStan-enabled-brightgreen.svg?style=flat)](https://github.com/phpstan/phpstan)

---

This repository (`phpstan/phpstan-src`) is for PHPStan's development only. Head to [`phpstan/phpstan`](https://github.com/phpstan/phpstan) for the main README, or to [create an issue](https://github.com/phpstan/phpstan/issues/new/choose).

## Contributing

Any contributions are welcome.

### Building

Initially you need to run `composer install`, or `composer update` in case you aren't working in a directory which was built before.

Afterwards you can either run the whole build including linting and coding standards using

```bash
vendor/bin/phing
```

### Running development version

You can also choose to run only part of the build. To analyse PHPStan by PHPStan itself, run:

```bash
vendor/bin/phing phpstan
```

### Fixing code style

To detect code style issues, run:

```bash
vendor/bin/phing cs
```

This requires PHP 7.4. On older versions the build target will be skipped and succeed silently.

And then to fix code style, run:

```bash
vendor/bin/phing cs-fix
```

### Running tests

Run:
```bash
vendor/bin/phing tests
```

### Debugging

1. Make sure XDebug is installed and configured.
2. Add `--xdebug` option when running PHPStan. Without it PHPStan turns the debugger off at runtime.

## Code of Conduct

This project adheres to a [Contributor Code of Conduct](https://github.com/phpstan/phpstan/blob/master/CODE_OF_CONDUCT.md).
By participating in this project and its community, you are expected to uphold this code.
