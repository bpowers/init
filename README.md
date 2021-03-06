[![Build Status](https://travis-ci.org/b1101/systemgo.svg?branch=master&bust=1)](https://travis-ci.org/b1101/systemgo)
[![Coverage Status](https://coveralls.io/repos/github/b1101/systemgo/badge.svg?branch=master&bust=1)](https://coveralls.io/github/b1101/systemgo?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/b1101/systemgo)](https://goreportcard.com/report/github.com/b1101/systemgo)
[![GoDoc](https://godoc.org/github.com/b1101/systemgo?status.svg)](https://godoc.org/github.com/b1101/systemgo)
[![GSoC Project abstract](http://b.repl.ca/v1/GSoC_Project-abstract-orange.png)](https://summerofcode.withgoogle.com/projects/#6227933760847872)
# Description
An init system in Go, intended to run on [Browsix](https://github.com/plasma-umass/browsix) and other Unix-like OS(GNU/Linux incl.)
# Features
* Fast and concurrent
* Handles dependencies well
* [Systemd](https://github.com/Systemd/Systemd)-compatible

# Milestones
- [x] `systemctl` can be used to `start` or `stop` units(_approx 10.07.2016_)
- [ ] _Systemgo_ functionality fully supported by [Browsix](https://github.com/plasma-umass/browsix)(_approx 20.07.2016_)
- [ ] A demo of a web service using _systemgo_ in the context of [Browsix](https://github.com/plasma-umass/browsix) is ready(_approx 01.08.2016_)
- [ ] `init` does not depend on HTTP for communication with `systemctl`

# Progress
- [x] Logging
- [x] Dependency resolution
    - [x] Wants
    - [x] Requires
    - [x] After
    - [x] Before
- [ ] Systemctl

# Supported Systemd functionality
## Commands
- [x] start
- [x] stop
- [ ] reload
- [x] restart
- [x] status
- [ ] isolate
- [ ] list-units
- [ ] enable
- [ ] disable

## Unit types
- [ ] Service
  - [x] Simple
  - [ ] Forking
  - [x] Oneshot
- [ ] Mount
- [x] Target
- [ ] Socket
