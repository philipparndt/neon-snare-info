# Privacy Policy — Apple TV

**Neon Snare for Apple TV**
Last updated: 26 July 2026

This is the policy for the **Apple TV** version. The iPhone and iPad version is
covered by [PRIVACY.md](PRIVACY.md). Both say the same thing about data
collection — there is none — and differ only in describing the two ends of the
iPhone-as-controller feature.

## The short version

Neon Snare collects no data about you. There is no analytics, no tracking, no
advertising, no account, and no third-party SDK of any kind. Nothing about you
leaves your home, because the game contains no code that talks to a server.

One thing is published, and only ever on your own local network: while Neon
Snare is open, **the Apple TV announces its own name** — the one you gave the
device in Settings, such as "Living Room" — so that an iPhone can find it and
act as the controller. That name is the only identifying value anywhere in this
game. It is described in full under
[The local network, and your Apple TV's name](#the-local-network-and-your-apple-tvs-name).

## What is stored, and where

The game saves a small amount of data **on your Apple TV**, using the standard
Apple mechanism for app preferences:

- your high scores and best-run statistics
- unlocked achievements and their progress
- your settings (music, sound effects, screen shake, challenge difficulty) and
  your last selected game mode, including whether two-player was co-op or versus

This never leaves the device. There is no iCloud sync, no Game Center, and no
server of mine holding a copy. If your Apple TV is backed up by Apple, this
data is included like any other app's — that backup belongs to you and is
governed by Apple's terms, not mine.

Deleting the app deletes all of it.

## The local network, and your Apple TV's name

Neon Snare lets an iPhone act as the controller for the Apple TV. For the two
to find each other, **the Apple TV announces itself on your local network**
while Neon Snare is open.

What it announces is:

- a service of type `_pulse-ctl._udp`
- **the name of your Apple TV** — whatever you called it in Settings, for
  example "Living Room". This is what appears in the list on the phone when you
  pick which Apple TV to connect to.

That name is the only identifying thing involved anywhere in this game, and it
is the name you chose yourself. It is broadcast on your local network only,
where every AirPlay-capable device already announces itself the same way. It is
never sent off your network, never stored by me, and never associated with
anything else, because there is nothing else.

The announcement also goes out over Apple's direct device-to-device Wi-Fi, so
the feature still works when the phone and the Apple TV are not on the same
Wi-Fi network. If your Apple TV asks for permission to access the local
network, this is what it is for.

## What crosses the link

Once a phone is connected, the two devices talk directly to each other. Nothing
passes through a server, and nothing is recorded on either end.

The **phone sends** only what a controller sends:

- how far your thumb has moved on the trackpad, and whether it is currently
  touching
- how many times you pressed select, back, or a direction
- which on-screen menu item you tapped
- a timestamp, echoed back so the game can measure and display the connection
  delay

The **Apple TV sends back** only what the phone needs in order to show a useful
controller:

- which kind of screen is currently open (menu, playing, paused, and so on)
- the labels of the menu items on that screen, so the phone can mirror them —
  these are the game's own text, such as "PLAY" or "SETTINGS"
- which item is currently highlighted
- short signals telling the phone when to vibrate

The phone does not send its name, its identifier, or anything about itself. If
you never use the controller feature, none of this happens.

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
