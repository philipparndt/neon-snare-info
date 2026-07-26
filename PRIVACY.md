# Privacy Policy

**Neon Snare for iPhone and iPad**
Last updated: 26 July 2026

The **Apple TV** version is covered by
[PRIVACY-APPLE-TV.md](PRIVACY-APPLE-TV.md). Both say the same thing about data
collection — there is none — and differ only in describing the two ends of the
iPhone-as-controller feature.

## The short version

Neon Snare collects no data about you. There is no analytics, no tracking, no
advertising, no account, and no third-party SDK of any kind. Nothing you do in
the game is sent anywhere, because the game has no way to send anything: it
contains no code that talks to a server.

## What is stored, and where

The game saves a small amount of data **on your device**, using the standard
Apple mechanism for app preferences:

- your high scores and best-run statistics
- unlocked achievements and their progress
- your settings (music, sound effects, frame rate, screen shake, challenge
  difficulty) and last selected game mode

This never leaves the device. It is not backed up to any server operated by
me. If your device backs itself up to iCloud or a computer, this data is
included in that backup like any other app's — that backup belongs to you and
is governed by Apple's terms, not mine.

Deleting the app deletes all of it.

## The local network permission

Neon Snare can use an iPhone as the controller for an Apple TV. iOS asks for
permission to access your **local network** the first time you open the
controller screen, because that is the only way for the two devices to find
each other.

When you use this feature:

- the iPhone looks for Apple TVs running Neon Snare, using Bonjour (service
  type `_pulse-ctl._udp`). Each Apple TV it finds announces **its own name** —
  whatever you called it in Settings, such as "Living Room" — and that is what
  the phone lists for you to pick from. That name is the only identifying thing
  anywhere in this game, it is one you chose yourself, and it travels no
  further than your local network.
- discovery also works over Apple's direct device-to-device Wi-Fi, so the two
  can find each other even when they are not on the same Wi-Fi network
- once connected, the phone sends only what a controller sends: where your
  thumb is on the trackpad and which buttons you pressed
- the Apple TV sends back only what the phone needs to show: which screen is
  open, its menu items, and short signals for haptic feedback

All of it stays on your local network and goes directly between your two
devices. It does not pass through any server, and none of it is recorded.

If you never use the controller feature, the permission is never requested.

## Children

The game is suitable for all ages and does not collect data from anyone,
including children.

## What I do not do

- No analytics or crash reporting SDKs
- No advertising or ad identifiers
- No user accounts, sign-in, or email collection
- No location, contacts, photos, microphone, or camera access
- No selling or sharing of data, because there is none to sell or share

## Support and questions

Questions about this policy, or anything else, are welcome in the
[issue tracker](../../issues).

## Changes

If this policy ever changes, the updated version will be published in this
repository, and its history is visible in the repository's commit log.
