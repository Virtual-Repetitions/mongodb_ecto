# Changelog

## Unreleased

* Introduce support for Ecto 3 (work in progress)
* Introduce GitHub actions, replacing Travis CI

## v0.1.4

  Support MongoDB version 3.2

## v0.1.3

  This version is limited to Ecto 1.0 because of known issues with 1.1

  * Additions:
    * Implement `count(field, :distinct)`

  * Bug fixes:
    * Handle models without autogenerated primary key on update and delete
    * Implement `Ecto.Adapter.stop/2` callback
    * Move encoding to adapter `load` and `dump` callbacks

## v0.1.2

  * Breaking changes:
    * Raise on `limit` and `offset` in `update_all` and `delete_all` queries,
      it's not supported by MongoDB, we were failing siletnly before

  * Bug fixes:
    * Allow interpolation in limit and offset

## v0.1.1

  * Bug fixes:
    * Fix logging issues on find queries

## v0.1.0

First release
