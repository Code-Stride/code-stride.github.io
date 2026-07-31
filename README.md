# code-stride.github.io

Serves `/.well-known/assetlinks.json` at the domain root.

Android only reads Digital Asset Links from the root of a host, so this file
cannot live in the VibeTube project-pages repo (which is served under
`/VibeTube/`). Without it, VibeTube share links open in a browser instead of
the app.

The fingerprint must match the key that signs release APKs. If the signing key
is ever rotated, add the new fingerprint here **before** shipping the build,
and keep the old one until those installs have updated.
