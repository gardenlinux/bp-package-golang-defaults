# Why is this package needed?
For the release of Garden Linux `2150.0.0`, the team decided to switch from go `1.24` to `1.25`. Debian used at that time `1.24` as default for go, so we needed to overwrite the `golang-defaults` package to ensure that the build process used `1.25` and not `1.24`.

In the meantime Debian updated from 1.24 to 1.26, so we archived `package-golang-defaults` and switched for the nightly to go version `1.26`. However the snapshot from 2150 still uses `1.24` as default, so this repository allows to create the needed backport packages to change the default go version to `1.26`.
