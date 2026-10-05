<!-- tyhp-readme:start -->
# tyhpdef/pusher-pusher-php-server

Tyhp type definitions for `pusher/pusher-php-server` `7.3.0`.

```bash
composer require --dev tyhpdef/pusher-pusher-php-server:7.3.0
```

This is a metapackage. Composer also installs `tyhpdef/pusher-pusher-php-server-impl` (type files).
Require **this** name, not `tyhpdef/pusher-pusher-php-server-impl`.

See https://tyhplang.com.

## Maintain `pusher/pusher-php-server`? Ship the types yourself

If you are a Packagist maintainer of `pusher/pusher-php-server`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/pusher-pusher-php-server-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `pusher/pusher-php-server` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/pusher-pusher-php-server": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `pusher/pusher-php-server` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `pusher/pusher-php-server` with a real constraint,
   `"replace": { "tyhpdef/pusher-pusher-php-server": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `pusher/pusher-php-server` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/pusher-pusher-php-server` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
