# Changelog

## [4.7.0](https://github.com/web3-storage/w3protocol/compare/access-api-v4.6.1...access-api-v4.7.0) (2023-01-19)


### Features

* upload-api-proxy production url is to aws http gateway instead of up.web3.storage ([#376](https://github.com/web3-storage/w3protocol/issues/376)) ([96a856d](https://github.com/web3-storage/w3protocol/commit/96a856dc7b8d9ed7d305e44d06579b16d629fa33))

## [4.6.1](https://github.com/web3-storage/w3protocol/compare/access-api-v4.6.0...access-api-v4.6.1) (2023-01-19)


### Bug Fixes

* debug logging describeFetch does not access `response.type` ([#373](https://github.com/web3-storage/w3protocol/issues/373)) ([d27b94c](https://github.com/web3-storage/w3protocol/commit/d27b94c9e7b685d62126c453734bf9d1cd6f2486))

## [4.6.0](https://github.com/web3-storage/w3protocol/compare/access-api-v4.5.0...access-api-v4.6.0) (2023-01-19)


### Features

* access-api proxy.js has configurable options.catchInvocationError, by default catches HTTPError -&gt; error result w/ status=502 ([#366](https://github.com/web3-storage/w3protocol/issues/366)) ([c8ca473](https://github.com/web3-storage/w3protocol/commit/c8ca4738dc5678b69e79cc70372bc69825c7026e))

## [4.5.0](https://github.com/web3-storage/w3protocol/compare/access-api-v4.4.0...access-api-v4.5.0) (2023-01-19)


### Features

* access-api createStoreProxy uses patched fetch that will log any non-ok responses (to debug) ([#364](https://github.com/web3-storage/w3protocol/issues/364)) ([e741bc0](https://github.com/web3-storage/w3protocol/commit/e741bc040ad78a65d9c329765bfd8aec7820d96f))

## [4.4.0](https://github.com/web3-storage/w3protocol/compare/access-api-v4.3.0...access-api-v4.4.0) (2023-01-18)


### Features

* access-api upload-api-proxy routes invocations with staging audience to staging upload-api ([#357](https://github.com/web3-storage/w3protocol/issues/357)) ([d8325af](https://github.com/web3-storage/w3protocol/commit/d8325afebde6c67fb54767a0ab1e639d6248389e))


### Bug Fixes

* upload-api-proxy default fetch binds to globalThis ([#361](https://github.com/web3-storage/w3protocol/issues/361)) ([a96e6af](https://github.com/web3-storage/w3protocol/commit/a96e6af1cebacb84a097d1fc24d4fe5f658c1b93))

## [4.3.0](https://github.com/web3-storage/w3protocol/compare/access-api-v4.2.0...access-api-v4.3.0) (2023-01-17)


### Features

* access-api forwards store/ and upload/ invocations to upload-api ([#334](https://github.com/web3-storage/w3protocol/issues/334)) ([b773376](https://github.com/web3-storage/w3protocol/commit/b77337692d9e4580031c429c429d4055d6f6ebff))

## [4.2.0](https://github.com/web3-storage/w3protocol/compare/access-api-v4.1.0...access-api-v4.2.0) (2022-12-15)


### Features

* **access-api:** access-api version endpoint has publicKey property ([#317](https://github.com/web3-storage/w3protocol/issues/317)) ([474d561](https://github.com/web3-storage/w3protocol/commit/474d561845f7c10a785421ef95e552385861a970))

## [4.1.0](https://github.com/web3-storage/w3protocol/compare/access-api-v4.0.0...access-api-v4.1.0) (2022-12-14)


### Features

* access-api version route sets did=ucantoServerId and adds a signer prop ([#305](https://github.com/web3-storage/w3protocol/issues/305)) ([5eab262](https://github.com/web3-storage/w3protocol/commit/5eab262d4bc503bf7a68f19b8193b3a57e5b8451))
* embedded key resolution ([#312](https://github.com/web3-storage/w3protocol/issues/312)) ([4da91d5](https://github.com/web3-storage/w3protocol/commit/4da91d5f7f798d0d46c4df2aaf224610a8760d9e))
* include ucanto server principal did as 'aud' key in /version endpoint ([#309](https://github.com/web3-storage/w3protocol/issues/309)) ([bf3b171](https://github.com/web3-storage/w3protocol/commit/bf3b17110b188c1326ba5b041d0f75906c793671))


### Bug Fixes

* access-api ctx.signer no longer uses env.DID. instead env.DID is only used for ucanto server id ([#303](https://github.com/web3-storage/w3protocol/issues/303)) ([93d7003](https://github.com/web3-storage/w3protocol/commit/93d70038abe1b36c2a84d10214143cda6b5e4423))
* access-api wrangler.toml sets DID env var in env.dev ([#297](https://github.com/web3-storage/w3protocol/issues/297)) ([c4ca459](https://github.com/web3-storage/w3protocol/commit/c4ca459445f902d65eade97f41a197fc9178636a))
* access-client/src/agent default PRINCIPAL is did:web:web3.storage ([#296](https://github.com/web3-storage/w3protocol/issues/296)) ([27f2f60](https://github.com/web3-storage/w3protocol/commit/27f2f60dac7c95cb9efd42a28f5abfef8bdeb197))
* add support for did:web in the cli ([#301](https://github.com/web3-storage/w3protocol/issues/301)) ([885f7c1](https://github.com/web3-storage/w3protocol/commit/885f7c15cec7a0724fcc4a8dd5eb0146a918373d))
* fix client cli service did resolve ([#292](https://github.com/web3-storage/w3protocol/issues/292)) ([6be9608](https://github.com/web3-storage/w3protocol/commit/6be9608a907665a8123938ef804bebfffc5c7232))
* use did:web key in root handler ([#311](https://github.com/web3-storage/w3protocol/issues/311)) ([537dc48](https://github.com/web3-storage/w3protocol/commit/537dc48f4d864d0dbe41752f1a45dd14cd03e489))

## [4.0.0](https://github.com/web3-storage/w3protocol/compare/access-api-v3.0.0...access-api-v4.0.0) (2022-12-13)


### ⚠ BREAKING CHANGES

* upgrade access-api @ucanto/* and @ipld/dag-ucan major versions ([#246](https://github.com/web3-storage/w3protocol/issues/246))
* access-client store decoupling ([#228](https://github.com/web3-storage/w3protocol/issues/228))
* upgrade to `@ucanto/{interface,principal}`@^4.0.0 ([#238](https://github.com/web3-storage/w3protocol/issues/238))
* follow up on the capabilities extract ([#239](https://github.com/web3-storage/w3protocol/issues/239))
* doc capabilities & make requierd nb non-optionals ([#159](https://github.com/web3-storage/w3protocol/issues/159))
* Remove 0.8 caps and add account delegation to the service ([#123](https://github.com/web3-storage/w3protocol/issues/123))
* bump to 0.9 ([#116](https://github.com/web3-storage/w3protocol/issues/116))

### Features

* [#153](https://github.com/web3-storage/w3protocol/issues/153) ([#177](https://github.com/web3-storage/w3protocol/issues/177)) ([d6d448c](https://github.com/web3-storage/w3protocol/commit/d6d448c16f188398c30f2d1b83f69e1d7becd450))
* access-api uses DID env variable when building its ucanto server id ([#275](https://github.com/web3-storage/w3protocol/issues/275)) ([311da78](https://github.com/web3-storage/w3protocol/commit/311da786b8f2fdf5ac585170e746a5a7b04ec57b))
* **access-client:** cli and recover ([#207](https://github.com/web3-storage/w3protocol/issues/207)) ([adb3a8d](https://github.com/web3-storage/w3protocol/commit/adb3a8d61d42b31f106e86b95faa3e442f5dc2c7))
* account recover with email ([#149](https://github.com/web3-storage/w3protocol/issues/149)) ([6c659ba](https://github.com/web3-storage/w3protocol/commit/6c659ba68d23c3448d5150bc76f1ddcb91ae18d8))
* bump to 0.9 ([#116](https://github.com/web3-storage/w3protocol/issues/116)) ([3e0b63f](https://github.com/web3-storage/w3protocol/commit/3e0b63f38aace3a86655a1aa40e529c1501dc136))
* doc capabilities & make requierd nb non-optionals ([#159](https://github.com/web3-storage/w3protocol/issues/159)) ([6496773](https://github.com/web3-storage/w3protocol/commit/6496773f2a4977e06126ade37ae9dfc218b05f7f))
* follow up on the capabilities extract ([#239](https://github.com/web3-storage/w3protocol/issues/239)) ([ef5e779](https://github.com/web3-storage/w3protocol/commit/ef5e77922b67155f0c3e5cb37c12e32f9a56cce1))
* Remove 0.8 caps and add account delegation to the service ([#123](https://github.com/web3-storage/w3protocol/issues/123)) ([878f8c9](https://github.com/web3-storage/w3protocol/commit/878f8c9a38f02dac509ef0b4437ab3d1b8467eb3)), closes [#117](https://github.com/web3-storage/w3protocol/issues/117) [#121](https://github.com/web3-storage/w3protocol/issues/121)
* Revert "feat!: upgrade to `@ucanto/{interface,principal}`@^4.0.0" ([#245](https://github.com/web3-storage/w3protocol/issues/245)) ([c182bbe](https://github.com/web3-storage/w3protocol/commit/c182bbe5e8c5a7d5c74b10cbf4b7a45b51e9b184))
* sync encode/decode delegations ([#276](https://github.com/web3-storage/w3protocol/issues/276)) ([ab981fb](https://github.com/web3-storage/w3protocol/commit/ab981fb6e33799153022c0f6d06c282917e7af7c))
* upgrade access-api @ucanto/* and @ipld/dag-ucan major versions ([#246](https://github.com/web3-storage/w3protocol/issues/246)) ([5e663d1](https://github.com/web3-storage/w3protocol/commit/5e663d12ccea7d21cc8e7c36869f144a08eaa1b0))
* upgrade to `@ucanto/{interface,principal}`@^4.0.0 ([#238](https://github.com/web3-storage/w3protocol/issues/238)) ([2f3bab8](https://github.com/web3-storage/w3protocol/commit/2f3bab8924fe7f34a5db64d2521730fc85739d3a))


### Bug Fixes

* 0.9 ([#78](https://github.com/web3-storage/w3protocol/issues/78)) ([1b1ed01](https://github.com/web3-storage/w3protocol/commit/1b1ed01d537e88bbdeb5ea2aeb967b27bd11f87d))
* add validation copy ([#257](https://github.com/web3-storage/w3protocol/issues/257)) ([7f50af4](https://github.com/web3-storage/w3protocol/commit/7f50af471aa5d4f50fc2ac92e7bcbcc311a800b4)), closes [#139](https://github.com/web3-storage/w3protocol/issues/139)
* fix Access API cannot get space/info [#243](https://github.com/web3-storage/w3protocol/issues/243) ([#255](https://github.com/web3-storage/w3protocol/issues/255)) ([1bacd54](https://github.com/web3-storage/w3protocol/commit/1bacd544da803c43cf85043ecdada4dee2b3e2d3))
* fix d1 migrations ([#264](https://github.com/web3-storage/w3protocol/issues/264)) ([fb8c09d](https://github.com/web3-storage/w3protocol/commit/fb8c09d5a243a20cbde2086eac57b9637a2e1d1d))
* make d1 spaces.metadata nullable and change to kysely ([#284](https://github.com/web3-storage/w3protocol/issues/284)) ([c8a9ce5](https://github.com/web3-storage/w3protocol/commit/c8a9ce544226b3c8456d45b15e29cec84894aeb8)), closes [#280](https://github.com/web3-storage/w3protocol/issues/280)
* make multiformats 9 go away ([#133](https://github.com/web3-storage/w3protocol/issues/133)) ([2668880](https://github.com/web3-storage/w3protocol/commit/2668880a23c28ee45596fb1bc978564908a17e18))
* miniflare dev script ([#137](https://github.com/web3-storage/w3protocol/issues/137)) ([1c5a4e2](https://github.com/web3-storage/w3protocol/commit/1c5a4e2f89018fdf1624cc41650764ee08f9adc4))
* testing staging deploy ([3d500fa](https://github.com/web3-storage/w3protocol/commit/3d500fa4e6cd17a1c0c9739fb3e0e722f97d599d))
* try to deploy api staging ([18b7b29](https://github.com/web3-storage/w3protocol/commit/18b7b296cb7e94c7fddeb163340cc0e72ce51c0a))
* try to deploy staging ([c616818](https://github.com/web3-storage/w3protocol/commit/c61681883e69982c5ae378e6ffbf54f45c397c89))


### Code Refactoring

* access-client store decoupling ([#228](https://github.com/web3-storage/w3protocol/issues/228)) ([a785278](https://github.com/web3-storage/w3protocol/commit/a7852785e2ac783bcb21790b4a87ee5ad0a1380e))

## [3.0.0](https://github.com/web3-storage/w3-protocol/compare/access-api-v2.0.1...access-api-v3.0.0) (2022-10-14)


### ⚠ BREAKING CHANGES

* new accounts (#72)
* awake (#66)

### Features

* **access-api:** add email notifications ([40b5332](https://github.com/web3-storage/w3-protocol/commit/40b53323b9c569b191f35d62d32aac844de18fdd))
* **access-api:** add logtail ([1246ab0](https://github.com/web3-storage/w3-protocol/commit/1246ab0846f49f9adce734cf4f651d22f7ac7536))
* **access-api:** add prod config ([60707ec](https://github.com/web3-storage/w3-protocol/commit/60707ecef6ed1af8d8fe38f9ee0deb9761cb80a6))
* **access-api:** new email template ([cc19320](https://github.com/web3-storage/w3-protocol/commit/cc193202e385d8079144aa90e989af07cf743b0b))
* awake ([#66](https://github.com/web3-storage/w3-protocol/issues/66)) ([bb66f57](https://github.com/web3-storage/w3-protocol/commit/bb66f5772049e3363a753ea5b336c2fa1e42911e))
* fail validate for register email and add metrics ([0916ba6](https://github.com/web3-storage/w3-protocol/commit/0916ba6bda8ad46ccc4f6bb0c6f4a48dd99db0c8))
* new accounts ([#72](https://github.com/web3-storage/w3-protocol/issues/72)) ([9f6cb41](https://github.com/web3-storage/w3-protocol/commit/9f6cb419d33b9446dd80f8541228096cf2677d45))
* resync ([5cae9cd](https://github.com/web3-storage/w3-protocol/commit/5cae9cd55cfcc06046eb23a2f33931299dd07ff5))
* sdk ([305b2d3](https://github.com/web3-storage/w3-protocol/commit/305b2d317ba4b8743a1594e9dbe0d22bac90c229))
* sdk and cli ([2373447](https://github.com/web3-storage/w3-protocol/commit/2373447db93ee16276f45fbfe40e4b98c28b6ab7))
* support ucan as bearer ([#50](https://github.com/web3-storage/w3-protocol/issues/50)) ([bc73755](https://github.com/web3-storage/w3-protocol/commit/bc73755a308d116ba42f67cef2c7a6be5307c327))
* update deps ([d276375](https://github.com/web3-storage/w3-protocol/commit/d2763750159ad56132f0b002ff5f50cc36fce20c))
* use modules and setup ([#99](https://github.com/web3-storage/w3-protocol/issues/99)) ([b060c0b](https://github.com/web3-storage/w3-protocol/commit/b060c0b299ee55dbe7820231c63be90129a39652)), closes [#98](https://github.com/web3-storage/w3-protocol/issues/98)


### Bug Fixes

* **access-api:** add kvs ([e241d62](https://github.com/web3-storage/w3-protocol/commit/e241d6290d93bfc20986591398ab20af6173ef78))
* **access-api:** add logtail to tests ([546152a](https://github.com/web3-storage/w3-protocol/commit/546152aea75aff393935d866cbd9c1a818e81725))
* **access-api:** add name to emails and fix miniflare dev ([ad84b46](https://github.com/web3-storage/w3-protocol/commit/ad84b4696ec9078800d4bb99597bc1da5068abc1)), closes [#60](https://github.com/web3-storage/w3-protocol/issues/60)
* **access-api:** changes names, update deps ([3f9e1f8](https://github.com/web3-storage/w3-protocol/commit/3f9e1f800728f57a9b194154c1b2e0133aa5bca4))
* **access-api:** ci tests ([314cf63](https://github.com/web3-storage/w3-protocol/commit/314cf635aa632e05a79822c5f7ec012559ff4427))
* **access-api:** cors on errors ([bb8e916](https://github.com/web3-storage/w3-protocol/commit/bb8e91693be87186846bac166b1e5ab05c33a112))
* **access-api:** test error in staging ([1a97a57](https://github.com/web3-storage/w3-protocol/commit/1a97a5797678d242db5849d9f10b8bc1907873d6))
* **access-api:** use different email for tests ([1a01504](https://github.com/web3-storage/w3-protocol/commit/1a0150429253afc572c9689f0a09a4c26499bd03))
* add analytics to staging and prod ([14941d9](https://github.com/web3-storage/w3-protocol/commit/14941d901e48e92896cc962b3e93488731afa381))
* add readme ([25a01f5](https://github.com/web3-storage/w3-protocol/commit/25a01f54c4db8f5af75e23c924d86a7a67823beb))
* add readme text ([088273e](https://github.com/web3-storage/w3-protocol/commit/088273e97a72f7ec85c60a5cb5dd6a8754603064))
* api ([4e70483](https://github.com/web3-storage/w3-protocol/commit/4e7048316d3ed95f5b7606830d75420c5020bf53))
* bump api ([88a381a](https://github.com/web3-storage/w3-protocol/commit/88a381ae2077d24ccd762dc7fb47f91a58268e89))
* change sentry name ([ad69e47](https://github.com/web3-storage/w3-protocol/commit/ad69e47cb01ad1acedccf95798eacd9a649659bd))
* fix ci ([ce8f7a9](https://github.com/web3-storage/w3-protocol/commit/ce8f7a937a336c6f86d22a25fe4a4465f0c86c58))
* new email for notifications ([57b6845](https://github.com/web3-storage/w3-protocol/commit/57b6845a56f534505eeabdf5ab2e20f8b37c9532))
* proper envs and update deps ([d5dccb6](https://github.com/web3-storage/w3-protocol/commit/d5dccb6e9c23b5ddbdffa4c67c04d195524b38f2))
* reconfigure ava to avoid ci problems ([ce2006e](https://github.com/web3-storage/w3-protocol/commit/ce2006eb8f02153618c2e483a5bb5983443ff89a))
* redirect on success ([#77](https://github.com/web3-storage/w3-protocol/issues/77)) ([0e67f3b](https://github.com/web3-storage/w3-protocol/commit/0e67f3be07118dd132770818486d2498416a300f))
* remove error ([1ba180b](https://github.com/web3-storage/w3-protocol/commit/1ba180b2c8a2da5dd9d3a69f23bcd93022500d6e))
* remove it@dag.house ([8d319fe](https://github.com/web3-storage/w3-protocol/commit/8d319fef315fa5dd3a0b88b8bf23f5576e8adc28))
* revert fail email validation ([389784b](https://github.com/web3-storage/w3-protocol/commit/389784bb995b18683ca71af63816db123880d3eb))
* route for staging ([8d5866f](https://github.com/web3-storage/w3-protocol/commit/8d5866f2bf870eaf2bb26bddef02ee8a0b6d1386))
* staging ([29db547](https://github.com/web3-storage/w3-protocol/commit/29db547848e8a5cab4d5c91a72010ed4aec5d09c))
* staging ([53f62b0](https://github.com/web3-storage/w3-protocol/commit/53f62b0269a7c3def5c22afb2b888d5886683f05))
* test api ([9597c44](https://github.com/web3-storage/w3-protocol/commit/9597c4486abb1c21a0d8a504d4bb8632581e4800))
* update readme ([2f78a93](https://github.com/web3-storage/w3-protocol/commit/2f78a930ef46b1e80d63f8e9b3bce6e960d5e4d9))

## [2.0.1](https://github.com/web3-storage/w3-protocol/compare/access-api-v2.0.0...access-api-v2.0.1) (2022-10-13)


### Bug Fixes

* **access-api:** add name to emails and fix miniflare dev ([ad84b46](https://github.com/web3-storage/w3-protocol/commit/ad84b4696ec9078800d4bb99597bc1da5068abc1)), closes [#60](https://github.com/web3-storage/w3-protocol/issues/60)
* bump api ([88a381a](https://github.com/web3-storage/w3-protocol/commit/88a381ae2077d24ccd762dc7fb47f91a58268e89))
* fix ci ([ce8f7a9](https://github.com/web3-storage/w3-protocol/commit/ce8f7a937a336c6f86d22a25fe4a4465f0c86c58))
* update readme ([2f78a93](https://github.com/web3-storage/w3-protocol/commit/2f78a930ef46b1e80d63f8e9b3bce6e960d5e4d9))

## [2.0.0](https://github.com/web3-storage/w3-protocol/compare/access-api-v1.0.0...access-api-v2.0.0) (2022-10-10)


### ⚠ BREAKING CHANGES

* new accounts (#72)

### Features

* new accounts ([#72](https://github.com/web3-storage/w3-protocol/issues/72)) ([9f6cb41](https://github.com/web3-storage/w3-protocol/commit/9f6cb419d33b9446dd80f8541228096cf2677d45))


### Bug Fixes

* redirect on success ([#77](https://github.com/web3-storage/w3-protocol/issues/77)) ([0e67f3b](https://github.com/web3-storage/w3-protocol/commit/0e67f3be07118dd132770818486d2498416a300f))

## [1.0.0](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.4.0...access-api-v1.0.0) (2022-09-21)


### ⚠ BREAKING CHANGES

* awake (#66)

### Features

* awake ([#66](https://github.com/web3-storage/ucan-protocol/issues/66)) ([bb66f57](https://github.com/web3-storage/ucan-protocol/commit/bb66f5772049e3363a753ea5b336c2fa1e42911e))
* support ucan as bearer ([#50](https://github.com/web3-storage/ucan-protocol/issues/50)) ([bc73755](https://github.com/web3-storage/ucan-protocol/commit/bc73755a308d116ba42f67cef2c7a6be5307c327))


### Bug Fixes

* **access-api:** cors on errors ([bb8e916](https://github.com/web3-storage/ucan-protocol/commit/bb8e91693be87186846bac166b1e5ab05c33a112))

## [0.4.0](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.3.0...access-api-v0.4.0) (2022-08-31)


### Features

* **access-api:** add email notifications ([40b5332](https://github.com/web3-storage/ucan-protocol/commit/40b53323b9c569b191f35d62d32aac844de18fdd))


### Bug Fixes

* new email for notifications ([57b6845](https://github.com/web3-storage/ucan-protocol/commit/57b6845a56f534505eeabdf5ab2e20f8b37c9532))
* reconfigure ava to avoid ci problems ([ce2006e](https://github.com/web3-storage/ucan-protocol/commit/ce2006eb8f02153618c2e483a5bb5983443ff89a))
* remove it@dag.house ([8d319fe](https://github.com/web3-storage/ucan-protocol/commit/8d319fef315fa5dd3a0b88b8bf23f5576e8adc28))

## [0.3.0](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.2.0...access-api-v0.3.0) (2022-08-30)


### Features

* fail validate for register email and add metrics ([0916ba6](https://github.com/web3-storage/ucan-protocol/commit/0916ba6bda8ad46ccc4f6bb0c6f4a48dd99db0c8))
* update deps ([d276375](https://github.com/web3-storage/ucan-protocol/commit/d2763750159ad56132f0b002ff5f50cc36fce20c))


### Bug Fixes

* add analytics to staging and prod ([14941d9](https://github.com/web3-storage/ucan-protocol/commit/14941d901e48e92896cc962b3e93488731afa381))
* revert fail email validation ([389784b](https://github.com/web3-storage/ucan-protocol/commit/389784bb995b18683ca71af63816db123880d3eb))

## [0.2.0](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.1.4...access-api-v0.2.0) (2022-08-26)


### Features

* **access-api:** add logtail ([1246ab0](https://github.com/web3-storage/ucan-protocol/commit/1246ab0846f49f9adce734cf4f651d22f7ac7536))
* **access-api:** new email template ([cc19320](https://github.com/web3-storage/ucan-protocol/commit/cc193202e385d8079144aa90e989af07cf743b0b))


### Bug Fixes

* **access-api:** add logtail to tests ([546152a](https://github.com/web3-storage/ucan-protocol/commit/546152aea75aff393935d866cbd9c1a818e81725))
* **access-api:** use different email for tests ([1a01504](https://github.com/web3-storage/ucan-protocol/commit/1a0150429253afc572c9689f0a09a4c26499bd03))

## [0.1.4](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.1.3...access-api-v0.1.4) (2022-08-25)


### Bug Fixes

* api ([4e70483](https://github.com/web3-storage/ucan-protocol/commit/4e7048316d3ed95f5b7606830d75420c5020bf53))
* route for staging ([8d5866f](https://github.com/web3-storage/ucan-protocol/commit/8d5866f2bf870eaf2bb26bddef02ee8a0b6d1386))
* staging ([29db547](https://github.com/web3-storage/ucan-protocol/commit/29db547848e8a5cab4d5c91a72010ed4aec5d09c))
* staging ([53f62b0](https://github.com/web3-storage/ucan-protocol/commit/53f62b0269a7c3def5c22afb2b888d5886683f05))

## [0.1.3](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.1.2...access-api-v0.1.3) (2022-08-25)


### Bug Fixes

* test api ([9597c44](https://github.com/web3-storage/ucan-protocol/commit/9597c4486abb1c21a0d8a504d4bb8632581e4800))

## [0.1.2](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.1.1...access-api-v0.1.2) (2022-08-25)


### Bug Fixes

* **access-api:** add kvs ([e241d62](https://github.com/web3-storage/ucan-protocol/commit/e241d6290d93bfc20986591398ab20af6173ef78))
* **access-api:** test error in staging ([1a97a57](https://github.com/web3-storage/ucan-protocol/commit/1a97a5797678d242db5849d9f10b8bc1907873d6))
* change sentry name ([ad69e47](https://github.com/web3-storage/ucan-protocol/commit/ad69e47cb01ad1acedccf95798eacd9a649659bd))
* proper envs and update deps ([d5dccb6](https://github.com/web3-storage/ucan-protocol/commit/d5dccb6e9c23b5ddbdffa4c67c04d195524b38f2))
* remove error ([1ba180b](https://github.com/web3-storage/ucan-protocol/commit/1ba180b2c8a2da5dd9d3a69f23bcd93022500d6e))

## [0.1.1](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.1.0...access-api-v0.1.1) (2022-08-24)


### Bug Fixes

* add readme ([25a01f5](https://github.com/web3-storage/ucan-protocol/commit/25a01f54c4db8f5af75e23c924d86a7a67823beb))
* add readme text ([088273e](https://github.com/web3-storage/ucan-protocol/commit/088273e97a72f7ec85c60a5cb5dd6a8754603064))

## [0.1.0](https://github.com/web3-storage/ucan-protocol/compare/access-api-v0.0.1...access-api-v0.1.0) (2022-08-24)


### Features

* **access-api:** add prod config ([60707ec](https://github.com/web3-storage/ucan-protocol/commit/60707ecef6ed1af8d8fe38f9ee0deb9761cb80a6))
* resync ([5cae9cd](https://github.com/web3-storage/ucan-protocol/commit/5cae9cd55cfcc06046eb23a2f33931299dd07ff5))
* sdk ([305b2d3](https://github.com/web3-storage/ucan-protocol/commit/305b2d317ba4b8743a1594e9dbe0d22bac90c229))
* sdk and cli ([2373447](https://github.com/web3-storage/ucan-protocol/commit/2373447db93ee16276f45fbfe40e4b98c28b6ab7))


### Bug Fixes

* **access-api:** changes names, update deps ([3f9e1f8](https://github.com/web3-storage/ucan-protocol/commit/3f9e1f800728f57a9b194154c1b2e0133aa5bca4))
* **access-api:** ci tests ([314cf63](https://github.com/web3-storage/ucan-protocol/commit/314cf635aa632e05a79822c5f7ec012559ff4427))
