# pile cast receiver

The Google Cast receiver of [pile](https://github.com/phoo-foo/pile), served at https://cast.phoo.foo.

Nothing is developed here. The receiver is built from pile's frontend and
published to the `gh-pages` branch of this repository by pile's CI on every
deploy. This branch only carries this file.

## What the receiver relies on

One receiver serves pile instances of different versions, so it uses only
these, and they stay stable:

- the handover message on the Cast channel `urn:x-cast:foo.phoo.pile`
- `GET /config` of the instance
- the live socket's `group` and `clock` channels
- the instance's database endpoint, for the group record
- the media URLs the instance hands out
