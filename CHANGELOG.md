# Changelog

All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.

## 1.1.0 (2020-10-31)


### Features

* **api:** add api to get connection stream without sending a ([5d720dd](https://github.com/dirvine/quic-p2p/commit/5d720dd3052a103152826c98e5a925f95343f3dc))
* **api:** change bootstrap_nodes arg in with_config API to be an slice rather than a VecDeque ([a505065](https://github.com/dirvine/quic-p2p/commit/a50506513a0f2623d0ae00a359b5d4ac167ccfb0))
* **api:** expose an async API ([5617cdd](https://github.com/dirvine/quic-p2p/commit/5617cdd1795c0e5a43f2da40fd31c1fdc8025181))
* **api:** refactor the API to allow reusing of streams to exchange ([097c0dc](https://github.com/dirvine/quic-p2p/commit/097c0dc236e224d365a757867e69ca426dc82288))
* **async-api:** add support for listening to messages from both uni-streams and bi-streams ([25d1163](https://github.com/dirvine/quic-p2p/commit/25d11637eb0941f06fd109144c539e7e27394232))
* **async-api:** expose a 'listen' API which return a stream of connections and in turn messages ([2bbfb21](https://github.com/dirvine/quic-p2p/commit/2bbfb21436637305a40c6b6fa4fd55c26693b9f8))
* **async-api:** expose a function to query remote address from a Connection ([3f624ba](https://github.com/dirvine/quic-p2p/commit/3f624ba1157a3d7269b9e398e22cd214780e4b7b))
* **async-api:** support for bootstrapping using multiple nodes concurrently ([8a07250](https://github.com/dirvine/quic-p2p/commit/8a072507fe40210600f2f0ce4dfac375ba7457f5))
* **async-api:** support sending a message on a Connection and awaiting for a response using unidirectional streams ([9b81728](https://github.com/dirvine/quic-p2p/commit/9b81728d92ce269756c825e426d54cabe9f67154))
* **audit:** add scheduled security audit scan ([d017920](https://github.com/dirvine/quic-p2p/commit/d0179202c27f7192daf0deed9c6540f9d96622d7))
* **header:** add message header that is sent over the wire for data ([4dc09b8](https://github.com/dirvine/quic-p2p/commit/4dc09b8b53c3557bb270d84b45e77872cc084394))


### Bug Fixes

* **client-ip:** set to use loopback ip if hard coded contacts are loopback ([06fb27f](https://github.com/dirvine/quic-p2p/commit/06fb27f7a24d4030029d1739746f18344c7b65b2))
* **endpoint:** return error if no local addr was specified and IGD is not available ([940dce9](https://github.com/dirvine/quic-p2p/commit/940dce912d96bbf61db3eae622587f4984c0d041))
* **log:** minor fixes in log messages ([0a9bf09](https://github.com/dirvine/quic-p2p/commit/0a9bf09f7a628843e014302e81d21070af5a5566))
* **port:** update qp2p endpoint port when a random port is used ([cfccd1c](https://github.com/dirvine/quic-p2p/commit/cfccd1ce04a9718aa4ba9723814323f0e6836b8a))
* **stream:** send the correct number of bytes to read/write usize from ([7e1820e](https://github.com/dirvine/quic-p2p/commit/7e1820eef2fac0e8b8ed5cadfdeb02c507e1a70e))
* **tests:** refactor and fix tests to use the new API ([8088adf](https://github.com/dirvine/quic-p2p/commit/8088adfdcf914152c845a5220c4762bcecee0ab8))
* handle key and certificate parse errors ([6e4cd2b](https://github.com/dirvine/quic-p2p/commit/6e4cd2b584e8eecb50ddffa35b18918b8cde7361))
* return error on connection failure ([43c844e](https://github.com/dirvine/quic-p2p/commit/43c844ed3aee702f561abe3ddc9fc9f5cfaf1c4b))

### [0.8.6](https://github.com/maidsafe/qp2p/compare/v0.8.5...v0.8.6) (2020-10-27)

### [0.8.5](https://github.com/maidsafe/qp2p/compare/v0.8.4...v0.8.5) (2020-10-26)

### [0.8.4](https://github.com/maidsafe/qp2p/compare/v0.8.3...v0.8.4) (2020-09-30)

### [0.8.3](https://github.com/maidsafe/qp2p/compare/v0.8.2...v0.8.3) (2020-09-24)

### [0.8.2](https://github.com/maidsafe/qp2p/compare/v0.8.1...v0.8.2) (2020-09-22)


### Features

* **api:** change bootstrap_nodes arg in with_config API to be an slice rather than a VecDeque ([a505065](https://github.com/maidsafe/qp2p/commit/a50506513a0f2623d0ae00a359b5d4ac167ccfb0))
* **header:** add message header that is sent over the wire for data ([4dc09b8](https://github.com/maidsafe/qp2p/commit/4dc09b8b53c3557bb270d84b45e77872cc084394))


### Bug Fixes

* **client-ip:** set to use loopback ip if hard coded contacts are loopback ([06fb27f](https://github.com/maidsafe/qp2p/commit/06fb27f7a24d4030029d1739746f18344c7b65b2))
* **endpoint:** return error if no local addr was specified and IGD is not available ([940dce9](https://github.com/maidsafe/qp2p/commit/940dce912d96bbf61db3eae622587f4984c0d041))
* **log:** minor fixes in log messages ([0a9bf09](https://github.com/maidsafe/qp2p/commit/0a9bf09f7a628843e014302e81d21070af5a5566))

### [0.8.1](https://github.com/maidsafe/qp2p/compare/v0.8.0...v0.8.1) (2020-09-08)
* Update repo/crate name to qp2p

### [0.8.0](https://github.com/maidsafe/qp2p/compare/0.7.0...v0.8.0) (2020-09-08)
* Update repo/crate name to quic_p2p to match org naming convention
* Refactor the API to allow reusing of streams to exchange multiple messages
* Refactor and fix tests to use the new API
* Add api to get connection stream without sending a message
* Update qp2p endpoint port when a random port is used
* Expose a function to query remote address from a Connection
* Add support for listening to messages from both uni-streams and bi-streams
* Expose a 'listen' API which return a stream of connections and in turn messages
* Support for bootstrapping using multiple nodes concurrently
* Support sending a message on a Connection and awaiting for a response using unidirectional streams
* Expose an async API

### [0.7.0]
* Standardize cargo dependency versioning
* Return an error when IGD fails

### [0.6.2]
* Fix clippy errors in feature-gated code
* Fix bug in get_connection_info with `upnp` enabled.

### [0.6.1]
* Skip port forwarding if quic-p2p is running on the loopback address.

### [0.6.0]
* Include support for UPnP and improve echo service.
* Use IGD for port forwarding and use the IGD gateway to find a node's local IP address.

### [0.5.0]
* Update quinn to 0.6.0
* Update rustls to 0.17.0

### [0.4.0]
* Force the use of the basic single-threaded Tokio scheduler to prevent conflicts when used by a crate using Tokio `rt-threaded` feature
* Take two channels, one for client event and a second one for a node
* Use node or client channel for sending a message depending on the peer we are receiving the message from
* Remove the use of peer certificate, and therefore remove it from the handshake process
* Use shared QUIC `ClientConfig` instead of one per peer
* Update for Rust 1.41 (mem::replace -> mem::take)
* Use structopt to parse command line arguments
* Rename `proxies` to `bootstrap_nodes`
* Migrate to async/await syntax with new quinn v0.5
* Update CI to run all packages in the worspace
* Migrate CI/CD pipeline to GitHub Actions
* Use new new-style macro import
* Unsent user messages in the pending queues of an ongoing connection attempt will now be sent back to the user library if the connection attempt fails.
* Report connection failure for all cases where the connection was initiated by us. Previously some of the cases where not handled.
* Fire unsent user messages to the clients back to the user library. Previously unsent messages to clients were silently ignored.

### [0.3.0]
* Expose `Dirs` and `OverRide` structs publicly.
* Add `boostrap_cache_dir` field to the config to specify a custom path for the bootstrap cache.

### [0.2.1]
* Fix incorrect deserialisation logic in `WireMsg`
* Fix `fmt::Display` for `Event` and `WireMsg`

### [0.2.0]
* Fix bugs
* Modify API and internals with changes required by routing
* Return user messages given via `send` API for both successful and unsuccessful sends
* Tie a user given token to the event returning the above message to help identify the context

### [0.1.1]
* Initial release.
* Implement bootstrap cache.
* Implement the bootstrap logic.
* Add peer types (Client/Node).
* Implement optimised user message transfer (for larger messages).
* Add utils for testing delayed connections.
* Add configuration loading from files and command line (with `structopt`).
