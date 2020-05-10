# php-coverage-checker

php-coverage-checker is a library for automated code coverage percentage checking with output coverage per file.

Initial commit is 100% the work of [Ocramius](https://github.com/ocramius): https://ocramius.github.io/blog/automated-code-coverage-check-for-github-pull-requests-with-travis/

## Installation

Composer!

`composer require --dev otis22/php-coverage-checker`

## Usage

1. Generate [XML Code Coverage](https://phpunit.de/manual/current/en/logging.html#logging.codecoverage.xml) using [PHPUnit](https://phpunit.de/manual/current/en/appendixes.configuration.html#appendixes.configuration.logging)
1. Run `vendor/bin/php-coverage-checker /path/to/clover.xml <minimum coverage percentage>`
    * e.g. `vendor/bin/php-coverage-checker build/clover.xml 100`

## Output

```
/home/runner/work/php-skelleton/php-skelleton/src/Test.php 100%
Code coverage is 100% - OK!
```
