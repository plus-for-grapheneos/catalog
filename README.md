# +PLUS catalog (staging)

The signed add-on catalog for +PLUS for GrapheneOS, served by GitHub Pages at
https://plus-for-grapheneos.github.io/catalog/.

- index.json lists the add-ons; index.json.sig is its RSA SHA-256 signature.
- models.json lists the on-device AI models (they are downloaded from their publishers); models.json.sig signs it.
- Each catalog carries its public key and an expiry date. A phone only accepts a catalog whose key matches the hash in
  its catalog link, whose signature checks, which has not expired, and whose serial is not older than the last one it saw.

This is a staging catalog for testing. Its key is not a release key.

## Source

- +PLUS, +PLUS AI and Phone+: https://github.com/plus-for-grapheneos (source being published).
- +PLUS bundles avbroot 3.37.0 and afsr 2.0.0, unchanged, GPL-3.0, by Andrew Gunnerson:
  https://github.com/chenxiaolong/avbroot and https://github.com/chenxiaolong/afsr.
- +PLUS AI bundles LiteRT-LM (Apache-2.0): https://github.com/google-ai-edge/LiteRT-LM.
- Phone+ (call screening) is based on the GrapheneOS Dialer (Apache-2.0) and bundles Mozilla Rhino 1.9.1
  (MPL-2.0): https://github.com/mozilla/rhino. Its licence notices are in the app (Settings > About).

+PLUS for GrapheneOS is an independent project, not affiliated with or endorsed by the GrapheneOS project.
