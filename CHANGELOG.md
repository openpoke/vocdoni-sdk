# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Credential service provider integrated
- Custom retry attempts and time for transactions waiting functionality
- Added `votesLeftCount` function for checking how many times a user can submit a vote

### Changed

- `header` and `streamUri` are no longer mandatory when creating an election.

## [0.0.3-alpha] - 2023-01-31

### Added

- Functionality to check if a user is in census `isInCensus`
- Functionality to check if a user has already voted `hasAlreadyVoted`
- Functionality to check if a user is able to vote `isAbleToVote`
- Export UMD version via `@vocdoni/sdk/umd`
- Deterministic Wallet generation from arbitrary data

### Fixed

- Return `voteId` when submitting vote instead of the transaction hash.
- `Buffer` imports for bundle
- Bundling & export issues

### Changed

- Removed `dvote-solidity` dependency.

## [0.0.2-alpha] - 2022-12-20

### Added

- Staging environment options for API and Faucet
- Functionality to end, pause, cancel and continue an election

### Fixed

- Fixed proof check using public key when signer is from type `Wallet`

### Changed

- Use voting endpoint instead of generic submitTx.
- Naming for client initialization options changed.
- There are now the new `UnpublishedElection` and `PublishedElection` classes
which extend from the abstract `Election` class.
- `fetchElection` accepts an election id.

## [0.0.1-alpha] - 2022-12-01

### Added

- First unstable version of the SDK for testing purposes

[0.0.3-alpha]: https://github.com/vocdoni/vocdoni-sdk/releases/tag/v0.0.3-alpha
[0.0.2-alpha]: https://github.com/vocdoni/vocdoni-sdk/releases/tag/v0.0.2-alpha
[0.0.1-alpha]: https://github.com/vocdoni/vocdoni-sdk/releases/tag/v0.0.1-alpha
