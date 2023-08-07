# IETF Multiformats Working Group

Multiformats are a collection of self-describing data formats that consist of an
inline data header and a data value. They are composable in that some of the
more complex forms take another multiformat header/value tuple as value,
recursively. Multiformats are designed to compose into binary streams with both
header values and data values expressed in unsigned varints (a slight variation
from protobuf varints and the UNIX LEB128 standard), with the exception of
multibase, which base-encodes any valid binary multiformat and prepends its
header to the target encoding rather than to the binary data value. The unsigned
varint-based binary multiformats include headers for cryptographic hashes
(multihash), cryptographic keys (multikey), network addresses (multiaddr), and a
variety of other binary serialization formats that do not meet all the
requirements to form part of the above registries (the rest of the
[multicodec][1] entries).

The scope of this Working Group is to discuss these formats as they relate to
standardization at the IETF. Specifically, the group is currently focused on the
standardization of the two most generally-useful Multiformats: Multibase and
Multihash. The input documents for these two Multiformats are:

* https://datatracker.ietf.org/doc/draft-multiformats-multibase/
* https://datatracker.ietf.org/doc/draft-multiformats-multihash/

Outputs for the group will be:

1. An RFC defining the unsigned varint primitive 
2. An RFC defining a registry-group for all the Multiformats, empty at
   inception, with registration process and group-wide constraints on
   registration values
3. An RFC defining the Multibase registry within the Multiformats registry
   group, empty at inception
4. A Multibase specification which populates the above with currently-stable and
   implemented registrations
5. An RFC defining the Multihash registry within the Multiformats registry
   group, empty at inception
6. A Multihash specification which populates the above with currently-stable and
   implemented registrations

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

[1]: https://ipfs.io/ipfs/QmXec1jjwzxWJoNbxQF5KffL8q6hFXm9QwUGaa3wKGk6dT/#title=Multicodecs&src=https://raw.githubusercontent.com/multiformats/multicodec/master/table.csv