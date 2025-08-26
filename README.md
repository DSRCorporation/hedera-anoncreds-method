# Hiero AnonCreds Method

The spec repository for the Hiero AnonCreds Method that describes management of AnonCreds resources on [Hedera Consensus Service (HCS)](https://hedera.com/consensus-service).

Read the spec: https://dsrcorporation.github.io/hedera-anoncreds-method/

Available implementations of Hiero AnonCreds:

- TypeScript: [Hiero DID SDK JS](https://github.com/hiero-ledger/hiero-did-sdk-js)
- Python: [Hiero DID SDK Python](https://github.com/hiero-ledger/hiero-did-sdk-python)

The specification uses [Spec-Up] format. For details on Spec-Up features and functionality please see [Spec-Up Documentation].

[Spec-Up]: https://github.com/decentralized-identity/spec-up
[Spec-Up Documentation]: https://identity.foundation/spec-up/

## Abstract

The Hiero AnonCreds Method specification defines how AnonCreds objects should be registered (written) and resolved when rooting them in a Hedera DID.
This specification parallels other DID-specific AnonCreds methods that are registered in the [AnonCreds Methods Registry](https://hyperledger.github.io/anoncreds-methods-registry/).

The specification leverages [HCS-1 standard](https://hashgraphonline.com/docs/standards/hcs-1/) for storing immutable files on Hedera Consensus Service (HCS).
All the published AnonCreds objects except for RevRegEntry are treated as HCS-1 files in this AnonCreds method (Schema, CredDef, RevRegDef).

For details about Hedera DIDs and how to write/read them, please see [Hedera DID Method specification](https://github.com/hashgraph/did-method).

## Contributing to the Specification

Pull requests (PRs) to this repository may be accepted.
Each commit of a PR must have a DCO (Developer Certificate of Origin -[https://github.com/apps/dco](https://github.com/apps/dco)) sign-off.

### Editing the spec locally

Editing the spec locally requires `npm` and `node` installed.

- Fork and locally clone the repository
- Run `npm install` from the repository root
- Edit the spec contents in the `/spec` folder
- Run `npm run render`
    - Alternatively, you can use `npm run edit` to enable interactive editing (rendered spec will be updated automatically as you apply changes)
- Open the resulting `index.html` file in a browser

## License

[Apache License 2.0](LICENSE)