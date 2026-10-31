# Super Shadowmount Plus FLZ by @FLZZilla

Public distribution repository for **Super Shadowmount Plus FLZ by @FLZZilla (SSMPlusFLZ)**.

This repository intentionally contains only public documentation, release metadata, and release verification automation. Development, patching, and build infrastructure are maintained separately in the private development repository.

## Credits and upstream

SSMPlusFLZ is built on top of **ShadowMountPlus by Drakmor**.

The core ShadowMount+ architecture, mounting logic, scanner, lifecycle handling, web/API functionality, PS5 integration, and continuing upstream development are Drakmor's work. SSMPlusFLZ adapts that foundation with EXLZ/FLZ-specific behavior and related compatibility fixes.

Please support and follow the original project:

- **Author / upstream maintainer:** Drakmor
- **Upstream:** https://github.com/drakmor/ShadowMountPlus
- **Upstream releases:** https://github.com/drakmor/ShadowMountPlus/releases


## Latest Release

<!-- latest-release:start -->
**Super Shadowmount Plus FLZ 1.7beta11 by @FLZZilla**

- Release: `1.7beta11-ssmplusflz-r15`
- Published: `2026-10-31`
- Binary: `supershadowmountplusflz.elf`
- SHA-256: `2857524bec1338d9caf1c7b22c75a026f683afa0eabdd9c947349e5cf221a679`
- Download: https://github.com/z3r3lkio/SSMPlusFLZ-Releases/releases/tag/1.7beta11-ssmplusflz-r15

<!-- latest-release:end -->

## Payload Manager source

This repository can be added directly as a custom source in **PS5 Payload Manager**.

Use this catalog URL:

```text
https://raw.githubusercontent.com/z3r3lkio/SSMPlusFLZ-Releases/main/payloads.json
```

In Payload Manager, open **Settings → Manage Sources → Add Source**, paste the URL above, and add it.

The catalog uses a stable payload ID so favorites and autoload entries survive version updates. It is updated automatically whenever a new Super Shadowmount Plus FLZ release is published and includes the current version, direct ELF download URL, release date, and SHA-256 checksum.

## Releases

Each public release inherits the corresponding Drakmor ShadowMountPlus version.

Example:

```text
Upstream:   1.7beta9
SSMPlusFLZ: 1.7beta9-ssmplusflz-rN
```

Public release assets include:

- `supershadowmountplusflz.elf`
- `supershadowmountplusflz.elf.sha256`
- a corresponding-source archive for the distributed binary

The public repository itself does **not** contain the private development history, internal build logic, patches, or development branches.

## What SSMPlusFLZ adds

- Folder-format LZ compatibility.
- `.exlz` images handled through the exFAT/LVD path.
- `.flz` images handled as PFSC containers like `.ffpfsc`.
- Recursive EXLZ/FLZ discovery beyond the normal directory scan depth.
- Preservation of standard scan roots when custom `scanpath=` entries are configured.
- Compatibility and safety fixes required by newer upstream releases.
- Stable binary name: **`supershadowmountplusflz.elf`**.

## License

The distributed software is based on GPL-licensed ShadowMountPlus. Corresponding source is made available with public binary releases.
