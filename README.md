<!-- tyhp-readme:start -->
# tyhpdef/league-config

Tyhp type definitions for `league/config` `1.2.0`.

```bash
composer require --dev tyhpdef/league-config:1.2.0
```

This is a metapackage. Composer also installs `tyhpdef/league-config-impl` (type files).
Require **this** name, not `tyhpdef/league-config-impl`.

See https://tyhplang.com.

## Maintain `league/config`? Ship the types yourself

If you are a Packagist maintainer of `league/config`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/league-config-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `league/config` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/league-config": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `league/config` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `league/config` with a real constraint,
   `"replace": { "tyhpdef/league-config": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `league/config` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/league-config` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
