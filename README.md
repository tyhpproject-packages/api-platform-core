<!-- tyhp-readme:start -->
# tyhpdef/api-platform-core

Tyhp type definitions for `api-platform/core` `4.4.0`.

```bash
composer require --dev tyhpdef/api-platform-core:4.4.0
```

This is a metapackage. Composer also installs `tyhpdef/api-platform-core-impl` (type files).
Require **this** name, not `tyhpdef/api-platform-core-impl`.

See https://tyhplang.com.

## Maintain `api-platform/core`? Ship the types yourself

If you are a Packagist maintainer of `api-platform/core`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/api-platform-core-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `api-platform/core` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/api-platform-core": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `api-platform/core` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `api-platform/core` with a real constraint,
   `"replace": { "tyhpdef/api-platform-core": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `api-platform/core` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/api-platform-core` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
