## Unreleased

## 0.2.6 - (October 26, 2018)
### Changed
* Use the `signal-hook` crate for managing signal registrations

## 0.2.5 - (September 29, 2018)
### Fixes
* Fix a possible starvation when polling multiple `Signal` instances outside of
a tokio reactor (e.g. by using `Future::wait`)

## 0.2.4 - (August 25, 2018)
### Fixes
* Actually make `unix::bsd` public

## 0.2.3 - (August 25, 2018)
### Features
* Exposes `SIGINFO` on BSD-based operating systems.

## 0.2.2 - (August 14, 2018)
### Fixes
* Fix starvation of `Signal`s whenever a `Signal` instance is dropped
* Fix starvation of individual `Signal`s based on their creation order

## 0.2.1 - (May 27, 2018)
### Fixes
* Bump minimum supported version of `mio` to 0.6.14

## 0.2.0 - (May 7, 2018)
#### Features
 * Uses `tokio` instead of `tokio_core`
 * Supports all 33 signals on FreeBSD
