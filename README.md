# Published installer QA

A public test harness for the already-public Miss You Dog installer. It contains only Windows installer checks. Application source and device credentials are not included.

The workflow uses a standard Windows GitHub-hosted runner, downloads the public installer, verifies its pinned SHA256, and checks native startup and window settings on a disposable VM. Logs contain test results only; no application profiles or private artifacts are uploaded.

An optional `MISSDOG_QA_BIND_CODE` Actions secret accepts a disposable, one-use test invite. The installed app redeems it through its real visible form and clicks the pet; only the generated test binding/event IDs are reported. No profile/token or artifact is uploaded, and the secret and binding are removed after the test.
