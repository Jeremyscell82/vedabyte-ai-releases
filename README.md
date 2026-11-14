# Vedabyte AI - Downloads

Public download home for **Vedabyte AI**, the private, on-device AI agent for macOS.

This repository holds release binaries only. The application source is private.

## Download

The latest notarized build is always here:

**https://github.com/Jeremyscell82/vedabyte-ai-releases/releases/latest**

Direct link (stable filename):

```
https://github.com/Jeremyscell82/vedabyte-ai-releases/releases/latest/download/VedabyteAI.dmg
```

Each release also carries a versioned DMG (`VedabyteAI-<version>.dmg`) and a
`SHA256SUMS.txt` so a download can be verified:

```bash
shasum -a 256 -c SHA256SUMS.txt
```

## Requirements

- Apple Silicon Mac (M-series)
- macOS 27 or later

Models download on demand inside the app; the DMG is small.

## Verify the app

Every build is signed with a Developer ID certificate, notarized by Apple, and
stapled, so it launches without a Gatekeeper warning. To check a download:

```bash
spctl -a -vvv -t exec "/Applications/Vedabyte AI.app"
xcrun stapler validate "/Applications/Vedabyte AI.app"
```

## Support

Questions, bug reports, or a build request: https://vedabyte.ai/contact
