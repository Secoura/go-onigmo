### go-oniguruma
This repository is a fork of [moovweb/rubex](https://github.com/moovweb/rubex/tree/go1) - a simple regular expression library (based on [oniguruma](https://github.com/kkos/oniguruma)) that supports Ruby's regex syntax.
The Rubex was originally created by Zhigang Chen (zhigang.chen@moovweb.com or zhigangc@gmail.com). It implements all the public functions of Go's Regexp package, except LiteralPrefix. By the benchmark tests in Regexp, the library is 40% to 10X faster than Regexp on all but one test. Unlike Go's Regrexp, this library supports named capture groups and also allow "\\1" and "\\k<name>" in replacement strings.
The library calls the Oniguruma regex library for regex pattern searching. All replacement code is done in Go.

To install everything (oniguruma and rubex), just run:
```sh
# linux (debian/ubuntu/...)
sudo apt-get install libonig-dev

# osx (homebrew)
brew install oniguruma

go install -i .
```