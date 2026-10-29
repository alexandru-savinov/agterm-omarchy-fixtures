# agterm Omarchy rendering fixtures

Two bounded, unchanged PNG references from an isolated native Omarchy ARM64 terminal test are stored through Git LFS.
See [fixture provenance and byte-verification instructions](rendering/omarchy-arm64/README.md).
The image pair totals 603,409 bytes; it is not a portable pixel-perfect golden test or a new runtime result.

The canonical application and acceptance evidence remain in [agterm-omarchy](https://github.com/alexandru-savinov/agterm-omarchy).
The [native evidence task](https://github.com/alexandru-savinov/agterm-omarchy/issues/22) preserves source/binary identity and cleanup corrections.
The [LFS verification task](https://github.com/alexandru-savinov/agterm-omarchy/issues/28) records actual transfer checks and account-access limitations.

This separate non-fork repository exists because GitHub rejected uploading new LFS objects to the public application fork.
The application fork's history, visibility, and upstream relationship were preserved.
No paid overage setting is enabled by this repository.

```sh
git clone https://github.com/alexandru-savinov/agterm-omarchy-fixtures.git
cd agterm-omarchy-fixtures
git lfs pull --include='rendering/omarchy-arm64/*.png' --exclude=''
```

Git LFS must be available to materialize image bytes; a pointer-only checkout is not a verified fixture download.
The fixture manifest records exact SHA256 object IDs and sizes.
