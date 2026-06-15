# HBrun Downloads

This repository holds public download metadata for HBrun product packages.

Large product files should be attached to GitHub Releases. Git history should
only contain lightweight files such as:

- release notes;
- checksums;
- public manifests;
- package index documents.

## Product Areas

```text
manifests/                 Public machine-readable indexes.
streamcore-sdk/<version>/  StreamCore SDK release notes and checksums.
streamgate/<version>/      StreamGate release notes and checksums.
```

## Distribution Rules

- Do not commit large SDK packages, installers, archives, AAR files, or
  XCFrameworks directly into Git.
- Use Release assets for downloadable packages.
- Keep file names stable and product-facing.
- Publish SHA256 checksums for every downloadable package.
- Keep the official website manifest as the public entry point for version
  checks and download links.

## Current Status

The repository is initialized for metadata and test manifests. Product package
assets will be added later through GitHub Releases.
