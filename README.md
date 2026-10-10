# go.firewatchpro.watch

Static site for FireWatch Pro tag links (2026-10-08). NFC tags are written as
`https://go.firewatchpro.watch/CheckIn?nfc_tag_id=FW-XXXXXX`.

- `.well-known/apple-app-site-association` - iPhone Universal Links (Base44 forces an empty file on firewatchpro.watch, so iPhones opened tags in Safari).
- `.well-known/assetlinks.json` - Android App Links (same fingerprints as the main domain).
- `index.html` / `404.html` - no app installed: forward to the same path on https://firewatchpro.watch.

- `Join/index.html` - smart invite link (2026-10-09). Invite emails point at `/Join/?invite=1&email=...`: the app opens it when installed (AASA `/Join*` + Android App Links), a computer goes on to the website sign-up, a phone without the app gets the right store button.
