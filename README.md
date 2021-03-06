# rikkeisoft/sonar-rules

[![Build Status](https://travis-ci.org/rikkeisoft/sonar-rules.svg?branch=master)](https://travis-ci.org/rikkeisoft/sonar-rules)
[![Coverage Status](https://coveralls.io/repos/github/rikkeisoft/sonar-rules/badge.svg?branch=master)](https://coveralls.io/github/rikkeisoft/sonar-rules?branch=master)
[![Code Climate](https://codeclimate.com/github/rikkeisoft/sonar-rules/badges/gpa.svg)](https://codeclimate.com/github/rikkeisoft/sonar-rules)
[![Issue Count](https://codeclimate.com/github/rikkeisoft/sonar-rules/badges/issue_count.svg)](https://codeclimate.com/github/rikkeisoft/sonar-rules)

Make documents about Sonar rules

## Requirements

* php >= 7.0

## Installation

```bash
$ git clone https://github.com/rikkeisoft/sonar-rules
$ composer install
```

## Usage

- You could specify your Sonar's credential in CLI arguments:

```bash
$ php bin/sonardoc rules:list -u <username> <language>
# Example
$ php bin/sonardoc rules:list -u huynq js
```

- Or you can set your Sonar's username and password in `.env`:

```bash
$ cp .env{.example,}
# Edit the value of .env to yours
$ php bin/sonardoc rules:list <language>
# Example
$ php bin/sonardoc rules:list js
```

## Build assets

- **Note**: [Yarn](https://yarnpkg.com/en/docs/install) have to be installed.

```bash
$ yarn install
$ yarn run prod
```

## Changelog

See all change logs in [CHANGELOG.md][changelog]

## Contributing

All code contributions must go through a pull request and approved by
a core developer before being merged. This is to ensure proper review of all the code.

Fork the project, create a feature branch, and send a pull request.

To ensure a consistent code base, you should make sure the code follows the [PSR-2][psr2].

If you would like to help take a look at the [list of issues][issues].

## License

This project is released under the MIT License.   
Copyright © 2017 Rikkeisoft Co. Ltd.,


[changelog]: https://github.com/rikkeisoft/sonar-rules/blob/master/CHANGELOG.md
[psr2]: https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md
[issues]: https://github.com/rikkeisoft/sonar-rules/issues
