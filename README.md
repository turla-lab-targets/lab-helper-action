# lab-helper-action

A minimal composite GitHub Action used as a fixture by the
[CI/CD Pipeline Compromise Lab](https://github.com/TurlaFSB/cicd-compromise-lab),
**scenario 04 — mutable action tag hijack**.

It stands in for any third-party deploy-helper action a workflow might
reference by a mutable tag (`uses: turla-lab-targets/lab-helper-action@v1`).

## Tags

- `v1.0.0` / `v1` — the benign, original action (a deploy echo).

The lab demonstrates how force-moving the `v1` tag to a later, compromised
commit silently changes what every consuming workflow runs on its next
trigger — without the consumer's workflow file changing at all.

**This repository exists only for security education. Every credential used
against it is a dummy value. It is never used to attack anything outside the
`turla-lab-targets` lab org.**
