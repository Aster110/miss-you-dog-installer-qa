# Published installer QA

A public test harness for the already-public Miss You Dog installer. It contains only Windows installer checks. Application source and device credentials are not included.

The workflow uses a standard Windows GitHub-hosted runner, downloads the public installer, verifies its pinned SHA256, and checks native startup and window settings on a disposable VM. Logs contain test results only; no application profiles or private artifacts are uploaded.
