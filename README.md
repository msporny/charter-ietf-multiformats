# IETF Multiformats Working Group

Multiformats are a collection of self-describing data formats that consist of an
inline data header and a data value. Multiformats have binary and text-based
representations and are used to express base encodings (multibase),
cryptographic hashes (multihash), cryptographic keys (multikey), network
addresses (multiaddr), and a variety of other binary serialization formats
(multicodec).

The scope of this Working Group is to discuss these formats as they relate to
standardization at the IETF. Specifically, the group is currently focused on the
standardization of two Multiformats: Multibase and Multihash. The input
documents for these two Multiformats are:

* https://datatracker.ietf.org/doc/draft-multiformats-multibase/
* https://datatracker.ietf.org/doc/draft-multiformats-multihash/

Outputs for the group will be:

* A Multibase specification
* A Multihash specification
* A registry for Multiformats with initial entries for Multibase and Multihash

The outputs from this Working Group are currently being used by various groups,
including the W3C Verifiable Credentials Working Group, W3C Decentralized
Identifiers Working Group, Conexxus Age Verification Working Group, W3C Dataset
Canonicalization and Hashing Working Group, GS1 Verifiable Credentials, and
online communities such as the W3C Credentials Community Group and
Interplanetary File System developer community. The Multiformats Working Group
will communicate progress and seek input and review from the Working Groups
listed in this section as well as other relevant groups as the work progresses.

Items that are out of scope for the group include:

* Standardizing Multiformats that are not explicitly listed in the charter.
* Creating or standardizing new data formats identified by a Multiformat byte
  header.
* Determining whether one data format is better than another data format.
* Changing current Multiformat header assignments in a way that breaks backward
  compatibility with production deployments.
