# s3a-wasm-dist

**Build output only.** This repo has prebuilt `wasm-pack --target web --release` artifacts of the
`s3a-wasm-snapshot` crate from [ashleycribb/s3a-storage](https://github.com/ashleycribb/s3a-storage).
Don't edit these files by hand. Change the source in s3a-storage, and new builds get published here.

- `vX.Y.Z/`: an immutable versioned build. Pin to a tag.
- `latest/`: the most recent passing build.

Every build passed a Node smoke test (new_session, record_human, record_ai, export_bytes,
from_bytes round-trip, export_delta) before it was published. Each version folder has `BUILD_INFO.txt` with
its source commit and SHA-256.

CDN: `https://cdn.jsdelivr.net/gh/ashleycribb/s3a-wasm-dist@v0.1.1/v0.1.1/s3a_wasm_snapshot.js`

License: Apache-2.0
