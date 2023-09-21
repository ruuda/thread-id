# v4.2.0

Released 2023-08-20.

 * Switch to `pthread_threadid_np` instead of `pthread_self` on Apple platforms.
   The latter was not guaranteed to be unique for the lifetime of the process.
 * Ensures compatibility with Rust 1.34.2 through 1.72.0.

Thanks to Charles Hubain for contributing to this release.

# v4.1.0

Released 2023-05-15.

 * Add support for the `wasm32-unknown-unknown` target.
 * Ensures compatibility with Rust 1.34.2 through 1.69.0.

Thanks to dAxpeDDa for contributing to this release.

# v4.0.0

Released 2021-03-24.

**Compatibility**:

 * The minimum supported Rust version is now 1.34.2.

Changes:

 * Bump `redox_syscall` dependency to v0.2.
 * Ensures compatibility with Rust 1.34.2 through 1.50.0.

Thanks to zonyitoo for contributing to this release.

# v3.3.0

Released 2018-03-23.

 * Bump `winapi` dependency to v0.3.
 * Add CI badges to crate metadata.
 * Ensures compatibility with Rust 1.8.0 through 1.24.0.

Thanks to Martin Geisler and Bastien Orivel for contributing to this release.

# v3.2.0

Released 2017-06-26.

 * Add support for the Redox operating system.
 * Ensures compatibility with Rust 1.8.0 through 1.18.0.

Thanks to Ian Douglas Scott for contributing to this release.

# v3.1.0

Released 2017-05-13.

 * Add the MIT license as an alternative to the Apache 2.0 license. This license
   change applies retroactively to all versions, this is only a metadata change.

# v3.0.0

Released 2016-10-29.

 * Depend on libc only on Unix-like environments, and on kernel32-sys only
   on Windows. This requires Rust 1.8 or later, hence the major version
   bump.

# v2.0.0

Released 2016-04-09.

 * Change ID type to `usize` to better reflect the underlying platform IDs.
   This is a breaking change.
 * Allow functions to be inlined to avoid call overhead.

Many thanks to Amanieu d'Antras for contributing to this release.

# v1.0.0

Released 2016-03-13.

Initial release with Windows and Linux support.
