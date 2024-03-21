# 🫧 Blobstr

**Blobs simply transmitted over relays**

_This is still a draft, and is subject to breaking changes_

Blobstr is a very simple protocol that describes ways to store and retrieve file archives or other immutable binary data in a sufficiently decentralized yet simple, modular, extensible way. It was created as a dead simple alternative for decentralized file sharing that is easy to implement and work with.

It works by establishing a very simple base URI/URL standard that gives programs all information they need to retrieve the file from any one of multiple provider options, and verify its integrity. Read [BLIP-01](BLIP-01.md) for more details.

## Motivation

There are other solutions out there for decentralized file archival. So why bother with this?

Some existing decentralized file ar alternatives _(such as IPFS)_ are great in some aspects. However, they have some downsides. For example, here are some downsides of IPFS:

- It is somewhat complex and monolithic, raising the barrier of entry for new programs and implementations.
- It does not integrate very well with existing and well-established protocols and systems (such as HTTP and existing network protocols, existing file systems, and better-established virtual currencies such as Bitcoin)
- Other issues, which are well illustrated in [this article](https://fiatjaf.com/d5031e5b.html)

Here are the main issues with the current approach and other alternatives:

- **Centralized media uploaders**: Generally works, but presents the following issues:
  - Adds centralization to Nostr.
  - There is no way to verify the file was not tampered with or modified.
- **IPFS**: IPFS is decentralized, but:
  - it is not easy to integrate with. (The protocol is complex)
  - does not integrate well with other Nostr NIPs
  - it is not flexible enough to support other use cases
  - brings many other issues, which are well illustrated in [this article](https://fiatjaf.com/d5031e5b.html)

## Use cases

- More decentralized Nostr media uploader services
- File integrity and tamper detection for Nostr clients.
- A gallery of photos that are stored on a local file system, and replicated across multiple personal servers
- A decentralized `npm`-like registry for software packages or git repositories
- Monetization of file access (e.g. Pay to download a book)
- Private caching servers for files (e.g. Save bandwidth and increase privacy by caching files to a personal server)
 
## Guiding Principles

- Keep things as simple as possible
- Reuse existing protocols, systems, and infrastructure as much as possible.
- Make specifications small and modular, with only the bare minimum needed to achieve a goal, so that we may have "simple building blocks" that 
- Integrate well with the Nostr, Bitcoin, and the Freedom Tech ecosystem

## How is this protocol organized?

This protocol is organized with `BLIP` specs (BLobstr Implementation Possibilities). Only [BLIP-01](BLIP-01.md) is mandatory, all other BLIPs are optional.

## Contributions

Contributions are welcome! Please feel free to submit a PR in this repo or [send a patch](https://git-send-email.io) to [daniel@daquino.me](mailto:daniel@daquino.me)
