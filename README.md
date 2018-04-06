# Embedded devices Working Group

> Coordination repository of the embedded devices Working Group (WG)

This repository [issue tracker] is used by the embedded WG to coordinate efforts towards making Rust
a great choice for embedded development.

[issue tracker]: https://github.com/rust-lang-nursery/embedded-wg/issues

## Vision

What is it that we really want? At a broad level:

- To improve the absolute quality (functionality, safety, performance) of embedded software in the
  wild.
- To improve the productivity of embedded software development teams, by reducing the tangible and
  intangible costs of achieving a level of quality.
- To improve the experience for programmers developing for embedded systems.
- To make embedded systems programming more accessible for people that are not already embedded
  systems developers.

## Roster

- [@dvc94ch][] (all things RISCV)
- [@dylanmckay][] (all things AVR)
- [@hannobraun]
- [@jamesmunns]
- [@japaric][] (lead)
- [@jcsoo]
- [@pftbest][] (all things MSP430)
- [@thejpster]

[@dvc94ch]: https://github.com/dvc94ch
[@dylanmckay]: https://github.com/dylanmckay
[@hannobraun]: https://github.com/hannobraun
[@jamesmunns]: https://github.com/jamesmunns
[@japaric]: https://github.com/japaric
[@jcsoo]: https://github.com/jcsoo
[@pftbest]: https://github.com/pftbest
[@thejpster]: https://github.com/thejpster

### Subprojects

* [AVR fork of Rust](https://github.com/avr-rust/)

### Contact

You can usually find the members of the embedded WG on the #rust-embedded channel (server:
irc.mozilla.org). Most of us use our GH usernames as our IRC nicknames, except for @jamesmunns who
uses the nickname bitshiftmask on IRC.

## On going community efforts

### [`embedded-hal`]

[`embedded-hal`]: https://github.com/japaric/embedded-hal

`embedded-hal` is a project that aims to build a standard set of traits (interfaces) for I/O
functionality common in embedded devices: Serial, I2C, etc. with the goal of serving as a base for
building reusable driver crates, crates to interface with external components like sensors.

There are plenty of traits that still need to be designed, in particular ones that involve async
I/O. Join the discussion and help us design the missing traits so that they'll fulfill your needs.

### [The weekly driver initiative][wd]

To put the `embedded-hal` to test and to expand the embedded crates.io ecosystem we are running the
weekly driver initiative. The goal is to release a new `no_std`, generic, `embedded-hal` driver
crate every one or two weeks.

There's lots of cool devices that would be great to have drivers for. Join the initiative and help
us grow the embedded crates.io ecosystem!

[wd]: https://github.com/rust-lang-nursery/embedded-wg/issues/39

### [Awesome embedded Rust][aer]

`Awesome embedded Rust` is a curated list of resources related to embedded programming in Rust with
the goal to provide a comprehensive collection of information and pointers to get going with
various microcontroller architectures as well as sensors and actors connected to them.

Help us to become even more awesome by contributing more information you've come across or written
yourself! Pull requests are most welcome.

[aer]: https://github.com/rust-embedded/awesome-embedded-rust

## Help wanted!

[These issues need your help!][hw]

[hw]: https://github.com/rust-lang-nursery/embedded-wg/issues?q=is%3Aissue+is%3Aopen+label%3Ahelp-wanted

## RFCs

When the team deems it necessary the RFC process may be used to make decisions or to design
processes, user interfaces, APIs, etc.

Learn more about the Rust's RFC process (which is the same as our own) [here][1].

To create an RFC, simply:
- clone this repo to your own personal one
- copy `0000-template.md` to `text/0000-my-feature.md` (where "my-feature" is
  descriptive. Don't assign an RFC number yet)
- fill in the details of your RFC in that file
- Open an pull request with this repository
