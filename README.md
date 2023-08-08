# IETF Multiformats Working Group

Multiformats are a collection of self-describing data formats that consist of an
inline data header and a data value. They are composable in that some of the
more complex forms take another multiformat header/value tuple as value,
recursively. Multiformats are designed to compose data into binary streams with
both inline header values (called [multicodecs][1]) and corresponding data
values, with the exception of multibase, which base-encodes any binary and
prepends its inline header to the target encoding rather than to the binary data
value being encoded.

The scope of this Working Group is to discuss these formats as they relate to
standardization at the IETF for wider and safer usage. Specifically, the group
is currently focused on the standardization of the two most generally-useful
multiformats: multibase and multihash. The input documents for these two
multiformats are:

* https://datatracker.ietf.org/doc/draft-multiformats-multibase/
* https://datatracker.ietf.org/doc/draft-multiformats-multihash/

Outputs for the group will be:

1. An RFC specifying multibase usage
2. An RFC defining an independent multibase registry and populating it with
   today's already-implemented stable and final values
3. An RFC defining a registry-group for all the multicodecs, empty at
   inception, with registration process and group-wide constraints on
   registration values
4. An RFC specifying multihash usage
5. An RFC defining a multihash registry within the multicodecs registry group
   and populating it with today's already-implemented stable and final values

The outputs from this Working Group are currently being used by various groups,
including the W3C Verifiable Credentials Working Group, W3C Decentralized
Identifiers Working Group, Conexxus Age Verification Working Group, W3C Dataset
Canonicalization and Hashing Working Group, GS1 Verifiable Credentials, and
online communities such as the W3C Credentials Community Group and
Interplanetary File System developer community. The Multiformats Working Group
will communicate progress and seek input and review from the Working Groups
listed in this section as well as other relevant groups as the work progresses.

Items that are out of scope for the group include:

* Standardizing other multiformats that are not explicitly listed in the
  charter.
* Creating or standardizing new data formats identified by a multicodec byte
  header.
* Determining whether one data format is better than another data format.
* Changing current multiformat header assignments in a way that breaks backward
  compatibility with production deployments.

[1]: https://ipfs.io/ipfs/QmXec1jjwzxWJoNbxQF5KffL8q6hFXm9QwUGaa3wKGk6dT/#title=Multicodecs&src=https://raw.githubusercontent.com/multiformats/multicodec/master/table.csv