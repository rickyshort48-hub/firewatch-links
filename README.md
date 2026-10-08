# go.firewatchpro.watch

Static site for FireWatch Pro tag links (2026-10-08). NFC tags are written as
`https://go.firewatchpro.watch/CheckIn?nfc_tag_id=FW-XXXXXX`.

- `.well-known/apple-app-site-association` - iPhone Universal Links (Base44 forces an empty file on firewatchpro.watch, so iPhones opened tags in Safari).
- `.well-known/assetlinks.json` - Android App Links (same fingerprints as the main domain).
- `index.html` / `404.html` - no app installed: forward to the same path on https://firewatchpro.watch.
