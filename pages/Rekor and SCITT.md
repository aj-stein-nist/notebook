topic:: [[Supply Chain]], [[Software Supply Chain]], [[SCITT]], [[Rekor]]

- I thought about this when the docs and associated Rekor server code was at or around commit [commit `c30c448`](https://github.com/sigstore/rekor/commit/c30c4487f1f68fcf26a24dadc3dcdecff4591aa0) or a little after the release of version 1.3.4.
- Is Rekor a fullish SCITT Transparency Service? Not quite.
	- Pluggable digital signatures and signing are not possible [sigstore/rekor#1724](https://github.com/sigstore/rekor/issues/1724)
	- There is no customizable registration policy [sigstore/rekor#1598](https://github.com/sigstore/rekor/issues/1598)