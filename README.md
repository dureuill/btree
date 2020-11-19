BTreeMap
========

BTreeMap extracted from std for the purpose of adding experimental methods without having to recompile all of rustc.

To enable compilation, did the following changes:

1. Moved mod.rs to lib.rs
2. Set the toolchain to nightly
3. Added the list of unstable features to lib.rs
4. Commented out all the rustc only attributes (rustc, stable, unstable, ...)
5. Removed "may_dangle" where it was present and accordingly removed unsafe from drop
